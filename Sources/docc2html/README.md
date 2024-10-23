<h2>docc2html
  <img src="http://zeezide.com/img/macro/MacroExpressIcon128.png"
           align="right" width="100" height="100" />
</h2>

Tool to convert "DocC" archives, a format to document Swift frameworks
and packages:
[Documenting a Swift Framework or Package](https://developer.apple.com/documentation/Xcode/documenting-a-swift-framework-or-package),
to a static HTML site.

## Usage

Example:

```bash
$ swift run docc2html ~/Downloads/SlothCreator.doccarchive /tmp/SlothCreator/docs
```

## TODO

- [ ] better templates
- [ ] refactor code into a proper type and module for easier reuse
- [ ] drop dependency on Macro
- [ ] support Mustache templates in the filesystem! (for customization & faster testing)

### Who

**docc2html** is brought to you by
the
[Always Right Institute](http://www.alwaysrightinstitute.com)
and
[ZeeZide](http://zeezide.de).
We like
[feedback](https://twitter.com/ar_institute),
GitHub stars,
cool [contract work](http://zeezide.com/en/services/services.html),
presumably any form of praise you can think of.

---

# ふろく：How to use in my environment

1. run swift environment on Docker

```bash
$ docker run -v C:/Users/HiranYu1/LocalFiles/repo/docc2html:/workspace -it swift:latest
```

2. then, your local folder is connected to /workspace in swift environment.
3. run command like this

```bash
$ /workspace/Sources/docc2html# swift run docc2html ../MSSDeviceBinding4-3-5-2.doccarchive ../results/mssDoc_4352
```

-> so you have to put target XXXX.docarchive file on C:/Users/HiranYu1/LocalFiles/repo/docc2html/Source directory

4. converted files are created on the direcotry you pointed in the command  
   ->ちゃんとできているかはわからないが、ある程度変換してくれているっぽい
