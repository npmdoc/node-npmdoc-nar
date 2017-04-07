# api documentation for  [nar (v0.3.40)](https://github.com/h2non/nar)  [![npm package](https://img.shields.io/npm/v/npmdoc-nar.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nar) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nar.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nar)
#### node.js application archive

[![NPM](https://nodei.co/npm/nar.png?downloads=true)](https://www.npmjs.com/package/nar)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nar/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nar_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nar/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nar/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nar/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tomas Aparicio"
    },
    "bin": {
        "nar": "./bin/nar"
    },
    "bugs": {
        "url": "https://github.com/h2non/nar/issues"
    },
    "dependencies": {
        "archiver": "^1.2.0",
        "array-unique": "^0.2.1",
        "cli-table": "^0.3.0",
        "colors": "^1.1.0",
        "commander": "^2.9.0",
        "findup-sync": "^0.2.1",
        "fw": "^0.1.0",
        "hu": "^0.1.0",
        "mkdirp": "^0.5.0",
        "ncp": "^2.0.0",
        "progress": "^1.1.8",
        "read": "^1.0.5",
        "request": "^2.67.0",
        "request-progress": "^0.3.1",
        "requireg": "^0.1.3",
        "resolve-tree": "^0.1.11",
        "rimraf": "^2.4.4",
        "tar": "^2.1.1"
    },
    "description": "node.js application archive",
    "devDependencies": {
        "LiveScript": "^1.3.0",
        "chai": "^1.9.1",
        "mocha": "^1.21.1",
        "node-static": "^0.7.3",
        "semver": "^4.3.4",
        "stubby": "github:h2non/stubby4node"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "da57ab8ffc1e69bb75898c0e1556e40b1a11c58f",
        "tarball": "https://registry.npmjs.org/nar/-/nar-0.3.40.tgz"
    },
    "engines": {
        "node": ">= 0.12"
    },
    "gitHead": "88ba14ebc11075e5da50ad20d29b2714acbfe053",
    "homepage": "https://github.com/h2non/nar",
    "keywords": [
        "node",
        "archive",
        "archiver",
        "packager",
        "package",
        "compress",
        "zip",
        "tarball",
        "gzip",
        "pkg",
        "jar",
        "tar",
        "nexe",
        "executable",
        "embedded",
        "exe",
        "portable"
    ],
    "license": "MIT",
    "main": "lib/nar",
    "maintainers": [
        {
            "name": "h2non",
            "email": "tomas@aparicio.me"
        }
    ],
    "name": "nar",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/h2non/nar.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.3.40"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nar](#apidoc.module.nar)
1.  [function <span class="apidocSignatureSpan">nar.</span>create (options)](#apidoc.element.nar.create)
1.  [function <span class="apidocSignatureSpan">nar.</span>createExec (options)](#apidoc.element.nar.createExec)
1.  [function <span class="apidocSignatureSpan">nar.</span>download (options)](#apidoc.element.nar.download)
1.  [function <span class="apidocSignatureSpan">nar.</span>extract (options)](#apidoc.element.nar.extract)
1.  [function <span class="apidocSignatureSpan">nar.</span>get (options)](#apidoc.element.nar.get)
1.  [function <span class="apidocSignatureSpan">nar.</span>install (options)](#apidoc.element.nar.install)
1.  [function <span class="apidocSignatureSpan">nar.</span>list (options)](#apidoc.element.nar.list)
1.  [function <span class="apidocSignatureSpan">nar.</span>run (options)](#apidoc.element.nar.run)
1.  object <span class="apidocSignatureSpan">nar.</span>utils
1.  string <span class="apidocSignatureSpan">nar.</span>VERSION

#### [module nar.utils](#apidoc.module.nar.utils)
1.  boolean <span class="apidocSignatureSpan">nar.utils.</span>isWin
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>addExtension (it)](#apidoc.element.nar.utils.addExtension)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>archiveName (nar)](#apidoc.element.nar.utils.archiveName)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>checksum (file, cb)](#apidoc.element.nar.utils.checksum)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>clone (obj)](#apidoc.element.nar.utils.clone)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>copy (file, dest, cb)](#apidoc.element.nar.utils.copy)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>copyBinary (file, dest, cb)](#apidoc.element.nar.utils.copyBinary)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>discoverPkg (dir)](#apidoc.element.nar.utils.discoverPkg)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>echo (it)](#apidoc.element.nar.utils.echo)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>env (it)](#apidoc.element.nar.utils.env)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>executableMsg (file)](#apidoc.element.nar.utils.executableMsg)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>exists (it)](#apidoc.element.nar.utils.exists)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>exit (code)](#apidoc.element.nar.utils.exit)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>extend (target)](#apidoc.element.nar.utils.extend)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>handleExit (cb)](#apidoc.element.nar.utils.handleExit)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>has ()](#apidoc.element.nar.utils.has)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>httpStatus (code)](#apidoc.element.nar.utils.httpStatus)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isArray ()](#apidoc.element.nar.utils.isArray)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isDir (it)](#apidoc.element.nar.utils.isDir)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isExecutable (path)](#apidoc.element.nar.utils.isExecutable)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isFile (it)](#apidoc.element.nar.utils.isFile)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isLink (it)](#apidoc.element.nar.utils.isLink)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isObject (x)](#apidoc.element.nar.utils.isObject)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isString (x)](#apidoc.element.nar.utils.isString)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>isUrl (it)](#apidoc.element.nar.utils.isUrl)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>keys (it)](#apidoc.element.nar.utils.keys)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>lines (it)](#apidoc.element.nar.utils.lines)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>logError (err, debug)](#apidoc.element.nar.utils.logError)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>mk (p, opts, made)](#apidoc.element.nar.utils.mk)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>next (callback)](#apidoc.element.nar.utils.next)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>now ()](#apidoc.element.nar.utils.now)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>once (cb)](#apidoc.element.nar.utils.once)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>random ()](#apidoc.element.nar.utils.random)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>read (it)](#apidoc.element.nar.utils.read)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>rename (orig, filename, cb)](#apidoc.element.nar.utils.rename)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>replaceEnvVars (str)](#apidoc.element.nar.utils.replaceEnvVars)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>resolvePkgPath (it)](#apidoc.element.nar.utils.resolvePkgPath)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>rm (p, options)](#apidoc.element.nar.utils.rm)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>stringify (it)](#apidoc.element.nar.utils.stringify)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>tmpdir (name)](#apidoc.element.nar.utils.tmpdir)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>toKb (it)](#apidoc.element.nar.utils.toKb)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>vals (obj)](#apidoc.element.nar.utils.vals)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>winBinaryScript (path)](#apidoc.element.nar.utils.winBinaryScript)
1.  [function <span class="apidocSignatureSpan">nar.utils.</span>write (path, data)](#apidoc.element.nar.utils.write)
1.  string <span class="apidocSignatureSpan">nar.utils.</span>EOL
1.  string <span class="apidocSignatureSpan">nar.utils.</span>arch
1.  string <span class="apidocSignatureSpan">nar.utils.</span>delimiter
1.  string <span class="apidocSignatureSpan">nar.utils.</span>platform



# <a name="apidoc.module.nar"></a>[module nar](#apidoc.module.nar)

#### <a name="apidoc.element.nar.create"></a>[function <span class="apidocSignatureSpan">nar.</span>create (options)](#apidoc.element.nar.create)
- description and source-code
```javascript
create = function (options){
  var errored, emitter, pkgPath, pkg, name, tmpPath, baseDir, file, output, clean, cleanError, onError, onEntry, onEnd, doCreate
, compressAll, compressPkg, compressDependencies, e;
  errored = false;
  emitter = new EventEmitter;
  options = apply(
  options);
  pkgPath = options.path;
  if (pkgPath) {
    pkg = read(
    pkgPath);
  }
  if (pkg) {
    options = applyPkgOptions(options, pkg);
  }
  if (!pkg) {
    throw new Error('Cannot find package.json');
  }
  name = pkg.name || 'unnamed';
  tmpPath = tmpdir(name);
  options.base = baseDir = dirname(
  pkgPath);
  file = getFilename(options, pkg);
  output = outputFile(file, options.dest);
  clean = function(){
    emitter.emit('message', 'Cleaning temporary directories');
    try {
      return rm(tmpPath);
    } catch (e$) {}
  };
  cleanError = function(){
    clean();
    try {
      return rm(output);
    } catch (e$) {}
  };
  onError = once(function(err){
    cleanError();
    if (!errored) {
      emitter.emit('error', err);
    }
    return errored = true;
  });
  onEntry = function(it){
    if (it) {
      return emitter.emit('entry', it);
    }
  };
  onEnd = function(){
    clean();
    if (!errored) {
      return emitter.emit('end', output);
    }
  };
  doCreate = function(){
    return next(function(){
      var narConfig, deps, basePkg, all, doCompression, onCompress;
      handleExit(
      cleanError);
      narConfig = narManifest(name, pkg);
      emitter.emit('start', narConfig);
      emitter.emit('info', narConfig);
      deps = function(done){
        return compressDependencies(tmpPath, baseDir, function(err, files){
          if (err) {
            return onError(
            err);
          }
          if (files) {
            narConfig.files = narConfig.files.concat(files);
          }
          return done();
        });
      };
      basePkg = function(done){
        var config;
        config = {
          dest: tmpPath,
          base: baseDir,
          name: name,
          patterns: options.patterns
        };
        return compressPkg(config, function(it){
          narConfig.files.push(
          it);
          return done();
        });
      };
      all = function(done){
        return compressAll(narConfig, done);
      };
      doCompression = function(done){
        mk(
        tmpPath);
        return fw.series([deps, basePkg, all], done);
      };
      onCompress = function(err){
        if (err) {
          return onError(
          err);
        }
        return onEnd();
      };
      return doCompression(
      onCompress);
    });
  };
  compressAll = function(narConfig, cb){
    var config, packAll, saveConfig, exec, addBinary;
    config = {
      name: file,
      dest: options.dest,
      patterns: ['*.tar', narFile],
      src: tmpPath,
      ext: 'nar',
      gzip: true
    };
    packAll = function(done){
      return pack(config).on('error', done).on('entry', onEntry).on('end', function(){
        return done();
      });
    };
    saveConfig = function(done){
      return writeConfig(narConfig, tmpPath, done);
    };
    exec = function(){
      return fw.series([saveConfig, packAll], cb);
    };
    addBinary = function(){
      var binaryPath, pkgInfo;
      binaryPath = options.binaryPath;
      if (!isFile(
      binaryPath)) {
        return onError(
        new Error("Binary path do not exists: " + binaryPath));
      }
      pkgInfo = {
        name: 'node',
        archive: 'node',
        dest: '.node/bin',
        type: 'binary'
      };
      emitter.emit('archive', pkgInfo);
      return copyBinary(binaryPath, tmpPath, function(err, file){
        if (err) {
          return onError(
          new Error("Error while copying the binary: " + err));
        }
        config.patterns.push(
        basename(
        file));
        onEntry(
        {
          name: pkgInfo.archive,
          type: pkgInfo.type,
          size: '10485760',
          sourcePath: binaryPath
        });
        return checksum(file, function(err, hash){
          pkgInfo.checksum = hash; ...
```
- example usage
```shell
...
dest: 'build/', // defaults to current directory
binary: true, // embed node binary to use it when run the archive
dependencies: true, // embed dependencies declared in package.json
devDependencies: true, // the same for dev dependencies
globalDependencies: ['npm', 'grunt-cli'] // and for globals :)
}

nar.create(options)
.on('error', function (err) {
  throw err
})
.on('info', function (nar) {
  console.log(nar.name)
})
.on('entry', function (file) {
...
```

#### <a name="apidoc.element.nar.createExec"></a>[function <span class="apidocSignatureSpan">nar.</span>createExec (options)](#apidoc.element.nar.createExec)
- description and source-code
```javascript
createExec = function (options){
  var emitter, dest, tmpPath, tmpDownload, nodeBinary, clean, onError, onDownloadError, onEntry, onEnd, onCreateEnd, onProgress,
onDownload, onDownloadEnd, getBinaryType, createExecutable;
  emitter = new EventEmitter;
  options = apply(
  options);
  dest = options.dest || process.cwd();
  tmpPath = tmpdir();
  tmpDownload = null;
  options.dest = tmpPath;
  nodeBinary = null;
  clean = function(){
    emitter.emit('message', 'Cleaning temporary directories');
    try {
      rm(
      tmpPath);
      if (tmpDownload) {
        return rm(
        tmpDownload);
      }
    } catch (e$) {}
  };
  onError = once(function(err){
    clean();
    return emitter.emit('error', err);
  });
  onDownloadError = function(err){
    return onError(
    err);
  };
  onEntry = function(it){
    if (it) {
      return emitter.emit('entry', it);
    }
  };
  onEnd = function(it){
    clean();
    return emitter.emit('end', it);
  };
  onCreateEnd = function(narPath){
    return createExecutable(
    narPath);
  };
  onProgress = function(status){
    return emitter.emit('progress', status);
  };
  onDownload = function(){
    return emitter.emit(
    'download');
  };
  onDownloadEnd = function(it){
    return emitter.emit('downloadEnd', it);
  };
  getBinaryType = function(){
    var os, arch;
    os = options.os, arch = options.arch;
    return os + "-" + arch;
  };
  createExecutable = function(nar){
    var narFile, narPath, narOutput, cleanExec, copyNodeBinary, copyDirectory, copyNarPkg, createTarball, createBinary, generate
, extractBinary, getDownloadUrl, downloadBinary;
    narFile = basename(nar, '.nar');
    narPath = join(dest, narFile) + '.run';
    narOutput = join(dest, narFile) + ("-" + getBinaryType() + ".nar");
    cleanExec = function(){
      rm(
      narPath);
      return clean();
    };
    copyNodeBinary = function(done){
      var binDir;
      binDir = join(tmpPath, 'bin');
      mk(
      binDir);
      return copyBinary(nodeBinary || process.execPath, binDir, done);
    };
    copyDirectory = function(dest){
      return function(dir, next){
        var name, orig, pkgDest;
        name = basename(
        dir);
        orig = join(dest, name);
        pkgDest = join(dest, name);
        return fs.exists(orig, function(exists){
          if (exists) {
            return next();
          }
          return fs.exists(pkgDest, function(exists){
            if (exists) {
              return next();
            }
            mk(
            pkgDest);
            return ncp(dir, pkgDest, copyOpts, next);
          });
        });
      };
    };
    copyNarPkg = function(done){
      var narDest, narPath, narManifest, doCopy;
      narDest = join(tmpPath, 'nar');
      narPath = join(__dirname, '..');
      narManifest = require(join(narPath, 'package.json'));
      doCopy = function(paths, done){
        return ncp(narPath, narDest, copyOpts, function(err){
          var depsDest;
          if (err) {
            return done(
            err);
          }
          depsDest = join(narDest, 'node_modules');
          return fw.each(paths, copyDirectory(
          depsDest), done);
        });
      };
      return resolveTree.manifest(narManifest, {
        basedir: narPath
      }, function(err, tree){
        var paths, rootPaths, parentPaths;
        if (err) {
          return cb(err);
        }
        paths = arrayUnique(
        resolveTree.flattenMap(tree, 'root'));
        rootPaths = paths.filter(function(it){
          return join(options.base, 'node_modules', basename(it)) === it;
        });
        parentPaths = arrayUnique(
        paths.filter(function(it){
          return rootPaths.indexOf(
          it) === -1;
        }).filter(function(it){
          return new RegExp("^" + narPath).test(it) === false;
        }).map(function(it){
          return relative(join(options.base, 'node_modules'), it).split('/').shift();
        }).map(function(it){
          return join(options.base, 'node_modules', it);
        }).filter(function(it){
          return rootPaths.indexOf( ...
```
- example usage
```shell
...
You can pass any configuration [options](#options) and the following options:

- **path** 'string' Path to package.json or application directory. Required
- **dest** 'string' Extract destination path. Default to random temporal directory
- **file** 'string' Archive file name. Default to package name + version, taken from 'package.json'
- **patterns** 'array' List of glob patterns to match files to include or exclude. See [node-glob](https://github.com/isaacs/node
-glob)

### nar.createExec(options)

Same as 'nar.create()', but this generate an executable binary-like archive

Aditional executable options supported are:

- **os** 'string' Node.js OS binary platform to embed. Detault to runtime OS
- **arch** 'string' Node.js OS binary architecture to embed. Default to runtime OS arch
...
```

#### <a name="apidoc.element.nar.download"></a>[function <span class="apidocSignatureSpan">nar.</span>download (options)](#apidoc.element.nar.download)
- description and source-code
```javascript
download = function (options){
  var ref$, url, dest, filename, auth, emitter, output, errored, createDest, clean, onError, onDownload, onEnd, onProgress, handler
, doDownload, e;
  ref$ = options = apply(
  options), url = ref$.url, dest = ref$.dest, filename = ref$.filename, auth = ref$.auth;
  emitter = new EventEmitter;
  output = join(dest, filename);
  errored = false;
  createDest = function(){
    if (!exists(
    dest)) {
      return mk(dest);
    }
  };
  clean = function(){
    try {
      return rm(output);
    } catch (e$) {}
  };
  onError = once(function(err, code){
    errored = true;
    clean();
    if (err) {
      return emitter.emit('error', err, code);
    }
  });
  onDownload = function(){
    return emitter.emit(
    'download');
  };
  onEnd = once(function(){
    if (!errored) {
      return emitter.emit('end', output);
    }
  });
  onProgress = function(it){
    return emitter.emit('progress', it);
  };
  handler = function(err, res, data){
    if (err) {
      return onError(
      err);
    } else if (res.statusCode >= 400) {
      return onError(new Error("Invalid response code: " + httpStatus(res.statusCode)), res.statusCode);
    } else if (!data) {
      return onError(
      new Error('Empty response'));
    }
  };
  doDownload = function(){
    return next(function(){
      var stream, http;
      onDownload();
      createDest();
      stream = fs.createWriteStream(
      output);
      stream.on('error', onError);
      http = request(options, handler);
      http.on('error', onError);
      return progress(http).on('progress', onProgress).pipe(stream).on('close', onEnd);
    });
  };
  try {
    doDownload();
  } catch (e$) {
    e = e$;
    onError(
    e);
  }
  return emitter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.extract"></a>[function <span class="apidocSignatureSpan">nar.</span>extract (options)](#apidoc.element.nar.extract)
- description and source-code
```javascript
extract = function (options){
  var ref$, path, dest, tmpdir, emitter, errored, clean, cleanError, onEnd, onEntry, onMsg, onError, extractor, extractorFn, copyBinFn
, createSymlinks, getExtractFiles, extractArchives, copyNarJson, setExecutionPerms, extractNar, extractTasks, doExtract, e;
  options == null && (options = {});
  ref$ = options = apply(
  options), path = ref$.path, dest = ref$.dest, tmpdir = ref$.tmpdir;
  emitter = new EventEmitter;
  errored = false;
  clean = function(){
    try {
      return rm(tmpdir);
    } catch (e$) {}
  };
  cleanError = function(){
    clean();
    try {
      if (dest !== process.cwd()) {
        return rm(dest);
      }
    } catch (e$) {}
  };
  onEnd = function(){
    clean();
    if (!errored) {
      return emitter.emit('end', options);
    }
  };
  onEntry = function(entry){
    if (entry) {
      return emitter.emit('entry', entry);
    }
  };
  onMsg = function(msg){
    if (msg) {
      return emitter.emit('message', msg);
    }
  };
  onError = function(err){
    cleanError();
    if (!errored) {
      emitter.emit('error', err);
    }
    return errored = true;
  };
  extractor = function(options, type){
    return function(done){
      var path, dest, createLink, processGlobalBinaries, extractEnd;
      path = options.path, dest = options.dest;
      if (/\/@[a-z0-9]+\//i.test(path)) {
        path = path.replace(/@[a-z0-9]+\//i, '');
      }
      if (!isFile(
      path)) {
        return onError(
        new Error('The given path is not a file'));
      }
      if (isExecutable(
      path)) {
        return onError(
        executableMsg(
        path));
      }
      createLink = function(name, path){
        var binPath, root, binDir, binFile;
        binPath = join(dest, path);
        if (isFile(
        binPath)) {
          if (root = findup('package.json', {
            cwd: dirname(
            binPath)
          })) {
            binDir = join(dirname(
            root), '../../../', 'bin');
            binFile = join(binDir, name);
            if (!isDir(
            binDir)) {
              mk(binDir);
            }
            if (isWin) {
              return write(binFile + ".cmd", winBinaryScript(
              binPath));
            } else {
              return symlinkSync(binPath, binFile);
            }
          }
        }
      };
      processGlobalBinaries = function(pkg){
        var bin, name, path, own$ = {}.hasOwnProperty, results$ = [];
        bin = pkg.bin;
        if (isString(
        bin)) {
          return createLink(pkg.name, bin);
        } else if (isObject(
        bin)) {
          for (name in bin) if (own$.call(bin, name)) {
            path = bin[name];
            if (path) {
              results$.push(createLink(name, path));
            }
          }
          return results$;
        }
      };
      extractEnd = function(){
        var pkg;
        if (type === 'global-dependency') {
          pkg = read(
          join(dest, 'package.json'));
          if (pkg) {
            processGlobalBinaries(
            pkg);
          }
        }
        return done();
      };
      return function(){
        if (!isDir(
        dest)) {
          mk(
          dest);
        }
        return unpack(
        options).on('error', onError).on('entry', onEntry).on('end', extractEnd);
      }();
    };
  };
  extractorFn = function(it){
    var options;
    options = {
      gzip: false,
      path: join(tmpdir, it.archive),
      dest: normalizePath(
      join(dest, it.dest)),
      checksum: it.checksum
    };
    return extractor(options, it.type);
  };
  copyBinFn = function(options){
    return function(done){
      var origin, target;
      origin = join(tmpdir, options.archive);
      target = normalizePath(
      join(dest, options.dest));
      if (!isDir(
      target)) {
        mk(target);
      }
      return copy(origin, target, done);
    };
  };
  createSymlinks = function(files){
    return function(done){
      var links, base, cwd, name, link, own$ = {}.hasOwnProperty;
      links = files.links;
      base = join(de ...
```
- example usage
```shell
...

Aditional executable options supported are:

- **os** 'string' Node.js OS binary platform to embed. Detault to runtime OS
- **arch** 'string' Node.js OS binary architecture to embed. Default to runtime OS arch
- **node** 'string' Node.js version to embed. Default to the current node runtime version

### nar.extract(options)
Fired events: 'end, error, entry, archive, message, info, start'

Extract archive files into an output directory

##### Options

- **path** 'string' Path to nar archive. Required
...
```

#### <a name="apidoc.element.nar.get"></a>[function <span class="apidocSignatureSpan">nar.</span>get (options)](#apidoc.element.nar.get)
- description and source-code
```javascript
get = function (options){
  var ref$, url, dest, filename, auth, emitter, output, errored, createDest, clean, onError, onDownload, onEnd, onProgress, handler
, doDownload, e;
  ref$ = options = apply(
  options), url = ref$.url, dest = ref$.dest, filename = ref$.filename, auth = ref$.auth;
  emitter = new EventEmitter;
  output = join(dest, filename);
  errored = false;
  createDest = function(){
    if (!exists(
    dest)) {
      return mk(dest);
    }
  };
  clean = function(){
    try {
      return rm(output);
    } catch (e$) {}
  };
  onError = once(function(err, code){
    errored = true;
    clean();
    if (err) {
      return emitter.emit('error', err, code);
    }
  });
  onDownload = function(){
    return emitter.emit(
    'download');
  };
  onEnd = once(function(){
    if (!errored) {
      return emitter.emit('end', output);
    }
  });
  onProgress = function(it){
    return emitter.emit('progress', it);
  };
  handler = function(err, res, data){
    if (err) {
      return onError(
      err);
    } else if (res.statusCode >= 400) {
      return onError(new Error("Invalid response code: " + httpStatus(res.statusCode)), res.statusCode);
    } else if (!data) {
      return onError(
      new Error('Empty response'));
    }
  };
  doDownload = function(){
    return next(function(){
      var stream, http;
      onDownload();
      createDest();
      stream = fs.createWriteStream(
      output);
      stream.on('error', onError);
      http = request(options, handler);
      http.on('error', onError);
      return progress(http).on('progress', onProgress).pipe(stream).on('close', onEnd);
    });
  };
  try {
    doDownload();
  } catch (e$) {
    e = e$;
    onError(
    e);
  }
  return emitter;
}
```
- example usage
```shell
...
- **headers** 'object' Define aditional HTTP request headers
- **strictSSL** 'boolean' Performs HTTP request with valid SSL servers. Defaults to 'false'
- **save** 'boolean' Save installed package as runtime dependency in 'package.json'. Default to 'false'
- **saveDev** 'boolean' Save installed package as development dependency in 'package.json'. Default to 'false'
- **savePeer** 'boolean' Save installed package as peer dependency in 'package.json'. Default to 'false'
- **global** 'boolean' Install package as global dependency. Default to 'false'

### nar.get(options)
Alias: 'download'

Fired events: 'end, error, download, progress'

Download archive from remote server.
It supports basic HTTP authentication and proxy
...
```

#### <a name="apidoc.element.nar.install"></a>[function <span class="apidocSignatureSpan">nar.</span>install (options)](#apidoc.element.nar.install)
- description and source-code
```javascript
install = function (options){
  var ref$, path, url, dest, clean, global, emitter, output, pkgInfo, tmp, cleanDir, onError, onEntry, onDownload, onProgress, onArchive
, onDownloadEnd, onEnd, onExtract, getInstallPath, copy, createBinDir, setExecutionPerms, createLink, createBinary, processBinaries
, extractor, downloader, doInstall, e;
  ref$ = options = apply(
  options), path = ref$.path, url = ref$.url, dest = ref$.dest, clean = ref$.clean, global = ref$.global;
  emitter = new EventEmitter;
  output = null;
  pkgInfo = {};
  tmp = tmpdir(
  path);
  cleanDir = function(){
    try {
      if (isDir(
      tmp)) {
        rm(tmp);
      }
      if (clean && output) {
        return rm(output);
      }
    } catch (e$) {}
  };
  onError = function(err, code, cmd){
    cleanDir();
    return emitter.emit('error', err, code, cmd);
  };
  onEntry = function(entry){
    if (entry) {
      return emitter.emit('entry', entry);
    }
  };
  onDownload = function(){
    return emitter.emit('download');
  };
  onProgress = function(it){
    return emitter.emit('progress', it);
  };
  onArchive = function(it){
    pkgInfo = it;
    return emitter.emit('archive', it);
  };
  onDownloadEnd = function(it){
    return emitter.emit('downloadEnd', it);
  };
  onEnd = function(output){
    save(
    options);
    cleanDir();
    return emitter.emit('end', output, options);
  };
  onExtract = function(it){
    if (options.dest === tmp) {
      return copy();
    } else {
      return onEnd(
      it);
    }
  };
  getInstallPath = function(){
    var dest;
    if (global) {
      dest = resolve('npm');
      if (dest) {
        return dest = join(dest, '../../../', pkgInfo.name || 'pkg');
      } else {
        return onError(
        new Error('Cannot resolve global installation path'));
      }
    } else {
      return dest = join(process.cwd(), 'node_modules', pkgInfo.name || 'pkg');
    }
  };
  copy = function(){
    var dest;
    dest = getInstallPath();
    if (!isDir(
    dest)) {
      mk(dest);
    }
    return ncp(tmp, dest, function(err){
      if (err) {
        return onError(
        err);
      }
      processBinaries(
      dest);
      return onEnd(
      {
        dest: dest
      });
    });
  };
  createBinDir = function(dir){
    if (!isDir(
    dir)) {
      return mk(dir);
    }
  };
  setExecutionPerms = function(file){
    try {
      return chmodSync(file, '775');
    } catch (e$) {}
  };
  createLink = function(binPath, dest){
    if (isWin) {
      return write(dest + ".cmd", winBinaryScript(
      binPath));
    } else {
      symlinkSync(binPath, dest);
      return setExecutionPerms(
      dest);
    }
  };
  createBinary = function(dest, path, name){
    var binPath, root;
    binPath = join(dest, path);
    if (isFile(
    binPath)) {
      if (global) {
        root = join(dest, '../../../', 'bin');
        createBinDir(root);
        return createLink(binPath, join(root, name));
      } else {
        root = join(dest, '../', '.bin');
        createBinDir(root);
        return createLink(binPath, join(root, name));
      }
    }
  };
  processBinaries = function(dest){
    var pkg, bin, name, path, own$ = {}.hasOwnProperty, results$ = [];
    pkg = join(dest, 'package.json');
    if (isFile(
    pkg)) {
      bin = (pkg = read(
      pkg)).bin;
      if (isString(
      bin)) {
        return createBinary(dest, bin, pkg.name);
      } else if (isObject(
      bin)) {
        for (name in bin) if (own$.call(bin, name)) {
          path = bin[name];
          if (path) {
            results$.push(createBinary(dest, path, name));
          }
        }
        return results$;
      }
    }
  };
  extractor = function(path){
    emitter.emit(
    'start');
    options.path = path;
    options.dest || (options.dest = tmp);
    return extract(
    options).on('error', onError).on('entry', onEntry).on('archive', onArchive).on('end', onExtract);
  };
  downloader = function(){
    if (!url) {
      options.url = path;
    }
    return download(
    options).on('download', onDownload).on('progress', onProgress).on('erro ...
```
- example usage
```shell
...

Read and parse a given .nar archive, emitting the 'entry' event for each existent file

##### Options

- **path** 'string' Path to nar archive. Required

### nar.install(options)
Fired events: 'end, download, downloadEnd, error, entry, start, progress'

Install archive as dependency in 'node_modules' directory.
It can aditionally download the archive from remote server

##### Options
...
```

#### <a name="apidoc.element.nar.list"></a>[function <span class="apidocSignatureSpan">nar.</span>list (options)](#apidoc.element.nar.list)
- description and source-code
```javascript
list = function (options){
  var ref$, path, gzip, emitter, ended, error, files, onError, onEnd, onEntry, onListener, parse;
  ref$ = apply(
  options), path = ref$.path, gzip = ref$.gzip;
  emitter = new EventEmitter;
  ended = false;
  error = false;
  files = [];
  onError = function(err){
    error = err;
    return emitter.emit('error', err);
  };
  onEnd = function(){
    ended = true;
    return emitter.emit('end', files);
  };
  onEntry = function(entry){
    files.push(
    entry);
    return emitter.emit('entry', entry);
  };
  onListener = function(name, fn){
    switch (name) {
    case 'error':
      if (error) {
        return fn(
        error);
      }
      break;
    case 'end':
      if (ended) {
        return fn(
        files);
      }
    }
  };
  parse = function(){
    return next(function(){
      var nar, entries, entryReader, emitEntries, parse, stream;
      nar = null;
      entries = {};
      if (!isFile(
      path)) {
        return onError(
        new Error('The given path is not a file'));
      }
      if (isExecutable(
      path)) {
        return onError(
        executableMsg(
        path));
      }
      entryReader = function(entry){
        var data;
        data = '';
        if (/\.nar\.json$/.test(entry.path)) {
          entry.on('data', function(it){
            return data += it.toString();
          });
          return entry.on('end', function(){
            return nar = JSON.parse(
            data);
          });
        } else {
          return entries[entry.path] = entry, entries;
        }
      };
      emitEntries = function(){
        emitter.emit('info', nar);
        return nar.files.forEach(function(file){
          return onEntry(
          {
            archive: file.archive,
            type: file.type,
            dest: file.dest,
            size: entries[file.archive] ? entries[file.archive].size : void 8,
            props: entries[file.archive] ? entries[file.archive].props : void 8
          });
        });
      };
      parse = tar.Parse();
      parse.on('error', onError);
      parse.on('entry', entryReader);
      parse.on('end', function(){
        if (!nar) {
          return onError(
          new Error('Invalid nar file'));
        }
        emitEntries();
        return onEnd();
      });
      stream = fs.createReadStream(
      path);
      stream.on('error', onError);
      if (gzip) {
        stream = stream.pipe(createGunzip());
      }
      return stream.pipe(parse);
    });
  };
  emitter.on('newListener', onListener);
  parse();
  return emitter;
}
```
- example usage
```shell
...

- **path** 'string' Path to nar archive. Required
- **dest** 'string' Extract destination path. Defaults to random temporal directory
- **args** 'object' Aditional argument to pass to hooks. Keys must have the same hook name
- **hooks** 'boolean' Enable/disable run command hooks. Defaults to 'true'
- **clean** 'boolean' Clean app directory on exit. Defaults to 'true'

### nar.list(options)
Options: 'path'

Fired events: 'end, error, entry'

Read and parse a given .nar archive, emitting the 'entry' event for each existent file

##### Options
...
```

#### <a name="apidoc.element.nar.run"></a>[function <span class="apidocSignatureSpan">nar.</span>run (options)](#apidoc.element.nar.run)
- description and source-code
```javascript
run = function (options){
  var ref$, path, hooks, args, dest, clean, emitter, cleanDir, onError, onEntry, onArchive, onProgress, onDownloadEnd, onEnd, onDownload
, hooksFn, appRunner, extractArchive, downloadArchive, doExtract, e;
  ref$ = options = apply(
  options), path = ref$.path, hooks = ref$.hooks, args = ref$.args, dest = ref$.dest, clean = ref$.clean;
  emitter = new EventEmitter;
  cleanDir = function(){
    try {
      if (clean) {
        return rm(dest);
      }
    } catch (e$) {}
  };
  onError = function(err, code, cmd){
    cleanDir();
    return emitter.emit('error', err, code, cmd);
  };
  onEntry = function(entry){
    if (entry) {
      return emitter.emit('entry', entry);
    }
  };
  onArchive = function(archive){
    if (archive) {
      return emitter.emit('archive', archive);
    }
  };
  onProgress = function(status){
    return emitter.emit('progress', status);
  };
  onDownloadEnd = function(it){
    return emitter.emit('downloadEnd', it);
  };
  onEnd = function(options, nar){
    cleanDir();
    return emitter.emit('end', options, nar);
  };
  onDownload = function(){
    return emitter.emit(
    'download');
  };
  hooksFn = function(nar){
    var buf, addHookFn, addStartMainScript, hook, ref$, cmd, own$ = {}.hasOwnProperty;
    buf = [];
    addHookFn = function(cmd, hook){
      if (args && has(args, hook) && args[hook]) {
        cmd += ' ' + parseFlags(
        isArray(
        args[hook])
          ? args[hook].join(' ')
          : args[hook]);
      }
      return buf.push(
      exec(emitter, cmd, dest, hook));
    };
    addStartMainScript = function(){
      if (nar.manifest.main) {
        return buf.push(
        exec(emitter, "node " + (nar.manifest.main || ''), dest, 'start'));
      }
    };
    for (hook in ref$ = getHooks(nar, args)) if (own$.call(ref$, hook)) {
      cmd = ref$[hook];
      if (hooks || (!hooks && hook === 'start')) {
        addHookFn(cmd, hook);
      }
    }
    if (!buf.length) {
      addStartMainScript();
    }
    return buf;
  };
  appRunner = function(options){
    var nar;
    nar = readNarJson(
    dest);
    emitter.emit('info', nar);
    setEnvironment(dest, nar.manifest);
    if (nar.binary) {
      extendPath(
      dest);
      if (!isBinaryValid(
      nar)) {
        return onError(
        new Error('Unsupported binary platform or processor'));
      }
    }
    return fw.series(hooksFn(
    nar), function(err){
      if (err) {
        return onError(
        err);
      }
      return onEnd(options, nar);
    });
  };
  extractArchive = function(){
    emitter.emit(
    'extract');
    return extract(
    options).on('error', onError).on('entry', onEntry).on('archive', onArchive).on('end', appRunner);
  };
  downloadArchive = function(){
    options.url = path;
    return download(
    options).on('download', onDownload).on('error', onError).on('progress', onProgress).on('end', function(it){
      options.path = it;
      onDownloadEnd(
      it);
      return extractArchive();
    });
  };
  doExtract = function(){
    return next(function(){
      if (!path) {
        return onError(
        new Error('Required archive path option'));
      }
      handleExit(
      cleanDir);
      if (isUrl(
      path)) {
        return downloadArchive();
      } else {
        return extractArchive();
      }
    });
  };
  try {
    doExtract();
  } catch (e$) {
    e = e$;
    onError(
    "Cannot run the archive: " + e);
  }
  return emitter;
}
```
- example usage
```shell
...

##### Options

- **path** 'string' Path to nar archive. Required
- **dest** 'string' Extract destination path. Default to random temporal directory
- **tmpdir** 'string' Temporal directory to use. Default to random temporal directory

### nar.run(options)
Fired events: 'end, error, entry, archive, command, info, start, stdout, stderr, exit'

Read, extract and run an application. It will read [command scripts][npm-scripts] hooks in 'package.json'

##### Options

- **path** 'string' Path to nar archive. Required
...
```



# <a name="apidoc.module.nar.utils"></a>[module nar.utils](#apidoc.module.nar.utils)

#### <a name="apidoc.element.nar.utils.addExtension"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>addExtension (it)](#apidoc.element.nar.utils.addExtension)
- description and source-code
```javascript
addExtension = function (it){
  if (it && !_.isUrl(
  it)) {
    if (!/.nar$/.test(it)) {
      it += '.nar';
    }
  }
  return it;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.archiveName"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>archiveName (nar)](#apidoc.element.nar.utils.archiveName)
- description and source-code
```javascript
archiveName = function (nar){
  var name, version;
  name = '';
  if (nar) {
    name += nar.name || 'unnamed';
    if (version = nar.manifest.version) {
      name += "-" + version;
    }
    if (nar.binary) {
      name += "-" + platform + "-" + arch;
    }
  }
  return name + ".nar";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.checksum"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>checksum (file, cb)](#apidoc.element.nar.utils.checksum)
- description and source-code
```javascript
checksum = function (file, cb){
  var hash;
  hash = crypto.createHash('sha1');
  return fs.createReadStream(
  file).on('data', (function(it){
    return hash.update(it);
  })).on('end', function(){
    return cb(null, hash.digest('hex'));
  }).on('error', cb);
}
```
- example usage
```shell
...
  extract = tar.Extract({
    path: dest
  });
  extract.on('entry', onEntry);
  return stream.pipe(extract).on('error', onError).on('end', onEnd);
};
calculateChecksum = function(hash, file, cb){
  return _.checksum(file, function(err, nhash){
    if (err) {
      return onError(
      err);
    }
    if (hash === nhash) {
      return cb();
    } else {
...
```

#### <a name="apidoc.element.nar.utils.clone"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>clone (obj)](#apidoc.element.nar.utils.clone)
- description and source-code
```javascript
function clone(obj) {
    return isArray(obj) ? obj.slice() : isObject(obj) ? extend({}, obj) : isDate(obj) ? new Date(obj.getTime()) : obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.copy"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>copy (file, dest, cb)](#apidoc.element.nar.utils.copy)
- description and source-code
```javascript
copy = function (file, dest, cb){
  var filename;
  filename = basename(
  file);
  dest = join(dest, filename);
  return fs.createReadStream(
  file).pipe(fs.createWriteStream(dest)).on('close', function(){
    return cb(null, dest);
  }).on('error', cb);
}
```
- example usage
```shell
...
  dest = join(dest, filename);
  return fs.createReadStream(
  file).pipe(fs.createWriteStream(dest)).on('close', function(){
    return cb(null, dest);
  }).on('error', cb);
},
copyBinary: function(file, dest, cb){
  return _.copy(file, dest, function(err, output){
    var name;
    if (err) {
      return cb(
      err);
    }
    if ((name = basename(
    file)) !== 'node') {
...
```

#### <a name="apidoc.element.nar.utils.copyBinary"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>copyBinary (file, dest, cb)](#apidoc.element.nar.utils.copyBinary)
- description and source-code
```javascript
copyBinary = function (file, dest, cb){
  return _.copy(file, dest, function(err, output){
    var name;
    if (err) {
      return cb(
      err);
    }
    if ((name = basename(
    file)) !== 'node') {
      return _.rename(output = join(dirname(
      output), name), 'node', function(err){
        if (err) {
          return cb(
          err);
        }
        return cb(null, output);
      });
    } else {
      return cb(null, output);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.discoverPkg"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>discoverPkg (dir)](#apidoc.element.nar.utils.discoverPkg)
- description and source-code
```javascript
discoverPkg = function (dir){
  dir == null && (dir = process.cwd());
  return findup('package.json', {
    cwd: dir
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.echo"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>echo (it)](#apidoc.element.nar.utils.echo)
- description and source-code
```javascript
echo = function (it){
  if (it) {
    return console.log.apply(this, arguments);
  } else {
    return console.log('');
  }
}
```
- example usage
```shell
...
    code);
  }
  return function(message){
    if (message != null) {
      if (String.prototype.red != null) {
        message = message.red;
      }
      _.echo(
      message);
    }
    return exit(
    code);
  };
},
read: function(it){
...
```

#### <a name="apidoc.element.nar.utils.env"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>env (it)](#apidoc.element.nar.utils.env)
- description and source-code
```javascript
env = function (it){
  return env[it] || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.executableMsg"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>executableMsg (file)](#apidoc.element.nar.utils.executableMsg)
- description and source-code
```javascript
executableMsg = function (file){
  file = basename(
  file || 'sample.nar');
  if (_.isWin) {
    return "the nar file is an executable, you cannot run it in Windows";
  } else {
    return "the nar file is an executable, you must run it as binary:\n\n  Example:\n  $ chmod +x " + file + "\n  $ ./" + file + "
exec --port 8080 --verbose\n\nYou could use the exec, start, extract, install or list commands\nFor more usage information, see the docs at github.com/h2non/nar";
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.exists"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>exists (it)](#apidoc.element.nar.utils.exists)
- description and source-code
```javascript
exists = function (it){
  return it && fs.existsSync(
  normalize(
  it));
}
```
- example usage
```shell
...
    copyDirectory = function(dest){
return function(dir, next){
  var name, orig, pkgDest;
  name = basename(
  dir);
  orig = join(dest, name);
  pkgDest = join(dest, name);
  return fs.exists(orig, function(exists){
    if (exists) {
      return next();
    }
    return fs.exists(pkgDest, function(exists){
      if (exists) {
        return next();
      }
...
```

#### <a name="apidoc.element.nar.utils.exit"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>exit (code)](#apidoc.element.nar.utils.exit)
- description and source-code
```javascript
exit = function (code){
  if (code === 0 || !code) {
    exit(
    code);
  }
  return function(message){
    if (message != null) {
      if (String.prototype.red != null) {
        message = message.red;
      }
      _.echo(
      message);
    }
    return exit(
    code);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.extend"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>extend (target)](#apidoc.element.nar.utils.extend)
- description and source-code
```javascript
function extend(target) {
    var origins = Array.prototype.slice.call(arguments, 1);
    var obj = isObject(target) ? target : {};
    origins.reduce(function (origin, o, index) {
        isObject(origin) ? keys(origin).forEach(function (name) {
            return obj[name] = origin[name];
        }) : void 0;
        return origins[index + 1];
    }, origins[0]);
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.handleExit"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>handleExit (cb)](#apidoc.element.nar.utils.handleExit)
- description and source-code
```javascript
handleExit = function (cb){
  var listener;
  listener = function(){
    process.stdin.resume();
    cb();
    return process.removeListener('SIGINT', listener);
  };
  return process.on('SIGINT', listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.has"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>has ()](#apidoc.element.nar.utils.has)
- description and source-code
```javascript
function has() {
    var args = Array.prototype.slice.call(arguments, 0);
    return curry(function (obj, prop) {
        return hasOwn.call(obj, prop);
    }).apply(void 0, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.httpStatus"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>httpStatus (code)](#apidoc.element.nar.utils.httpStatus)
- description and source-code
```javascript
httpStatus = function (code){
  if (code) {
    return code + " " + (status[code] || '');
  } else {
    return '';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.isArray"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isArray ()](#apidoc.element.nar.utils.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.isDir"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isDir (it)](#apidoc.element.nar.utils.isDir)
- description and source-code
```javascript
isDir = function (it){
  return _.exists(
  it) && fs.lstatSync(
  normalize(
  it)).isDirectory();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.isExecutable"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isExecutable (path)](#apidoc.element.nar.utils.isExecutable)
- description and source-code
```javascript
isExecutable = function (path){
  var buffer, num, data;
  buffer = new Buffer(25);
  num = fs.readSync(fs.openSync(path, 'r'), buffer, 0, 25, 0);
  data = buffer.toString('utf-8', 0, num);
  return /^\#\!\/bin\/bash/.test(data) && /\#\#nar\#\#/.test(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.isFile"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isFile (it)](#apidoc.element.nar.utils.isFile)
- description and source-code
```javascript
isFile = function (it){
  return _.exists(
  it) && (fs.lstatSync(
  normalize(
  it)).isFile() || _.isLink(
  it));
}
```
- example usage
```shell
...
},
stringify: function(it){
  if (it) {
    return JSON.stringify(it, null, 2);
  }
},
resolvePkgPath: function(it){
  if (_.isFile(
  it)) {
    return _.resolvePkgPath(
    dirname(
    it));
  } else {
    return it;
  }
...
```

#### <a name="apidoc.element.nar.utils.isLink"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isLink (it)](#apidoc.element.nar.utils.isLink)
- description and source-code
```javascript
isLink = function (it){
  return fs.lstatSync(
  normalize(
  it)).isSymbolicLink();
}
```
- example usage
```shell
...
  normalize(
  it)).isSymbolicLink();
},
isFile: function(it){
  return _.exists(
  it) && (fs.lstatSync(
  normalize(
  it)).isFile() || _.isLink(
  it));
},
random: function(){
  return _.now() + Math.floor(Math.random() * 10000);
},
lines: function(it){
  if (it) {
...
```

#### <a name="apidoc.element.nar.utils.isObject"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isObject (x)](#apidoc.element.nar.utils.isObject)
- description and source-code
```javascript
function isObject(x) {
    return toStr(x) === '[object Object]';
}
```
- example usage
```shell
...
    dirname(
    it));
  } else {
    return it;
  }
},
keys: function(it){
  if (hu.isObject(
  it)) {
    return Object.keys(
    it);
  } else {
    return [];
  }
},
...
```

#### <a name="apidoc.element.nar.utils.isString"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isString (x)](#apidoc.element.nar.utils.isString)
- description and source-code
```javascript
function isString(x) {
    return toStr(x) === '[object String]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.isUrl"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>isUrl (it)](#apidoc.element.nar.utils.isUrl)
- description and source-code
```javascript
isUrl = function (it){
  return /^http[s]?\:/.test(
  it);
}
```
- example usage
```shell
...
tmpdir: function(name){
  name == null && (name = 'pkg');
  name = basename(name, extname(
  name));
  return join(os.tmpdir(), "nar-" + name + "-" + _.random());
},
addExtension: function(it){
  if (it && !_.isUrl(
  it)) {
    if (!/.nar$/.test(it)) {
      it += '.nar';
    }
  }
  return it;
},
...
```

#### <a name="apidoc.element.nar.utils.keys"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>keys (it)](#apidoc.element.nar.utils.keys)
- description and source-code
```javascript
keys = function (it){
  if (hu.isObject(
  it)) {
    return Object.keys(
    it);
  } else {
    return [];
  }
}
```
- example usage
```shell
...
  } else {
    return it;
  }
},
keys: function(it){
  if (hu.isObject(
  it)) {
    return Object.keys(
    it);
  } else {
    return [];
  }
},
tmpdir: function(name){
  name == null && (name = 'pkg');
...
```

#### <a name="apidoc.element.nar.utils.lines"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>lines (it)](#apidoc.element.nar.utils.lines)
- description and source-code
```javascript
lines = function (it){
  if (it) {
    return it.split(os.EOL);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.logError"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>logError (err, debug)](#apidoc.element.nar.utils.logError)
- description and source-code
```javascript
logError = function (err, debug){
  if (err) {
    if (debug && err.stack) {
      return err.stack;
    } else {
      return ("Error: " + (err.message || err)).red;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.mk"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>mk (p, opts, made)](#apidoc.element.nar.utils.mk)
- description and source-code
```javascript
function sync(p, opts, made) {
    if (!opts || typeof opts !== 'object') {
        opts = { mode: opts };
    }

    var mode = opts.mode;
    var xfs = opts.fs || fs;

    if (mode === undefined) {
        mode = _0777 & (~process.umask());
    }
    if (!made) made = null;

    p = path.resolve(p);

    try {
        xfs.mkdirSync(p, mode);
        made = made || p;
    }
    catch (err0) {
        switch (err0.code) {
            case 'ENOENT' :
                made = sync(path.dirname(p), opts, made);
                sync(p, opts, made);
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                var stat;
                try {
                    stat = xfs.statSync(p);
                }
                catch (err1) {
                    throw err0;
                }
                if (!stat.isDirectory()) throw err0;
                break;
        }
    }

    return made;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.next"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>next (callback)](#apidoc.element.nar.utils.next)
- description and source-code
```javascript
function nextTick(callback) {
  if (typeof callback !== 'function')
    throw new TypeError('callback is not a function');
  // on the way out, don't bother. it won't get fired anyway.
  if (process._exiting)
    return;

  var args;
  if (arguments.length > 1) {
    args = new Array(arguments.length - 1);
    for (var i = 1; i < arguments.length; i++)
      args[i - 1] = arguments[i];
  }

  nextTickQueue.push({
    callback,
    domain: process.domain || null,
    args
  });
  tickInfo[kLength]++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.now"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>now ()](#apidoc.element.nar.utils.now)
- description and source-code
```javascript
now = function (){
  return Date.now();
}
```
- example usage
```shell
...
rm: rm.sync,
mk: mk.sync,
next: nextTick,
env: function(it){
  return env[it] || null;
},
now: function(){
  return Date.now();
},
isWin: platform === 'win32',
toKb: function(it){
  if (it) {
    return Math.round(it / 1024) || 1;
  } else {
    return 0;
...
```

#### <a name="apidoc.element.nar.utils.once"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>once (cb)](#apidoc.element.nar.utils.once)
- description and source-code
```javascript
once = function (cb){
  var error;
  error = false;
  return function(it){
    if (!error) {
      cb.apply(this, arguments);
    }
    if (it) {
      return error = true;
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.random"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>random ()](#apidoc.element.nar.utils.random)
- description and source-code
```javascript
random = function (){
  return _.now() + Math.floor(Math.random() * 10000);
}
```
- example usage
```shell
...
    return [];
  }
},
tmpdir: function(name){
  name == null && (name = 'pkg');
  name = basename(name, extname(
  name));
  return join(os.tmpdir(), "nar-" + name + "-" + _.random());
},
addExtension: function(it){
  if (it && !_.isUrl(
  it)) {
    if (!/.nar$/.test(it)) {
      it += '.nar';
    }
...
```

#### <a name="apidoc.element.nar.utils.read"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>read (it)](#apidoc.element.nar.utils.read)
- description and source-code
```javascript
read = function (it){
  var data;
  if (_.exists(
  it)) {
    data = fs.readFileSync(
    normalize(
    it)).toString();
    if (/.json$/.test(
    it)) {
      return JSON.parse(
      data);
    } else {
      return data;
    }
  } else {
    return null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.rename"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>rename (orig, filename, cb)](#apidoc.element.nar.utils.rename)
- description and source-code
```javascript
rename = function (orig, filename, cb){
  var base;
  base = dirname(
  orig);
  return fs.rename(orig, join(base, filename), cb);
}
```
- example usage
```shell
...
    return cb(null, hash.digest('hex'));
  }).on('error', cb);
},
rename: function(orig, filename, cb){
  var base;
  base = dirname(
  orig);
  return fs.rename(orig, join(base, filename), cb);
},
copy: function(file, dest, cb){
  var filename;
  filename = basename(
  file);
  dest = join(dest, filename);
  return fs.createReadStream(
...
```

#### <a name="apidoc.element.nar.utils.replaceEnvVars"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>replaceEnvVars (str)](#apidoc.element.nar.utils.replaceEnvVars)
- description and source-code
```javascript
replaceEnvVars = function (str){
  return str.replace(/\$\{(\w+)\}/ig, function(_, name){
    return process.env[name] || '';
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.resolvePkgPath"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>resolvePkgPath (it)](#apidoc.element.nar.utils.resolvePkgPath)
- description and source-code
```javascript
resolvePkgPath = function (it){
  if (_.isFile(
  it)) {
    return _.resolvePkgPath(
    dirname(
    it));
  } else {
    return it;
  }
}
```
- example usage
```shell
...
  if (it) {
    return JSON.stringify(it, null, 2);
  }
},
resolvePkgPath: function(it){
  if (_.isFile(
  it)) {
    return _.resolvePkgPath(
    dirname(
    it));
  } else {
    return it;
  }
},
keys: function(it){
...
```

#### <a name="apidoc.element.nar.utils.rm"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>rm (p, options)](#apidoc.element.nar.utils.rm)
- description and source-code
```javascript
function rimrafSync(p, options) {
  options = options || {}
  defaults(options)

  assert(p, 'rimraf: missing path')
  assert.equal(typeof p, 'string', 'rimraf: path should be a string')
  assert(options, 'rimraf: missing options')
  assert.equal(typeof options, 'object', 'rimraf: options should be object')

  var results

  if (options.disableGlob || !glob.hasMagic(p)) {
    results = [p]
  } else {
    try {
      options.lstatSync(p)
      results = [p]
    } catch (er) {
      results = glob.sync(p, options.glob)
    }
  }

  if (!results.length)
    return

  for (var i = 0; i < results.length; i++) {
    var p = results[i]

    try {
      var st = options.lstatSync(p)
    } catch (er) {
      if (er.code === "ENOENT")
        return

      // Windows can EPERM on stat.  Life is suffering.
      if (er.code === "EPERM" && isWindows)
        fixWinEPERMSync(p, options, er)
    }

    try {
      // sunos lets the root user unlink directories, which is... weird.
      if (st && st.isDirectory())
        rmdirSync(p, options, null)
      else
        options.unlinkSync(p)
    } catch (er) {
      if (er.code === "ENOENT")
        return
      if (er.code === "EPERM")
        return isWindows ? fixWinEPERMSync(p, options, er) : rmdirSync(p, options, er)
      if (er.code !== "EISDIR")
        throw er

      rmdirSync(p, options, er)
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.stringify"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>stringify (it)](#apidoc.element.nar.utils.stringify)
- description and source-code
```javascript
stringify = function (it){
  if (it) {
    return JSON.stringify(it, null, 2);
  }
}
```
- example usage
```shell
...
        }
      }
    }
  }
  return writeJson(pkgPath, pkg);
};
writeJson = function(path, pkg){
  return write(path, JSON.stringify(pkg, null, 2));
};
...
```

#### <a name="apidoc.element.nar.utils.tmpdir"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>tmpdir (name)](#apidoc.element.nar.utils.tmpdir)
- description and source-code
```javascript
tmpdir = function (name){
  name == null && (name = 'pkg');
  name = basename(name, extname(
  name));
  return join(os.tmpdir(), "nar-" + name + "-" + _.random());
}
```
- example usage
```shell
...
    return [];
  }
},
tmpdir: function(name){
  name == null && (name = 'pkg');
  name = basename(name, extname(
  name));
  return join(os.tmpdir(), "nar-" + name + "-" + _.random());
},
addExtension: function(it){
  if (it && !_.isUrl(
  it)) {
    if (!/.nar$/.test(it)) {
      it += '.nar';
    }
...
```

#### <a name="apidoc.element.nar.utils.toKb"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>toKb (it)](#apidoc.element.nar.utils.toKb)
- description and source-code
```javascript
toKb = function (it){
  if (it) {
    return Math.round(it / 1024) || 1;
  } else {
    return 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.vals"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>vals (obj)](#apidoc.element.nar.utils.vals)
- description and source-code
```javascript
function vals(obj) {
    return keys(obj).map(function (key) {
        return (obj || 0)[key];
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.winBinaryScript"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>winBinaryScript (path)](#apidoc.element.nar.utils.winBinaryScript)
- description and source-code
```javascript
winBinaryScript = function (path){
  path = normalize(
  path);
  return "@ECHO OFF\n@IF EXIST \"%~dp0\\node.exe\" (\n  \"%~dp0\\node.exe\" \"" + path + "\" %*\n) ELSE (\n  node \"" + path + "\" %*\n)";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nar.utils.write"></a>[function <span class="apidocSignatureSpan">nar.utils.</span>write (path, data)](#apidoc.element.nar.utils.write)
- description and source-code
```javascript
write = function (path, data){
  if (path) {
    return fs.writeFileSync(path, data);
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
