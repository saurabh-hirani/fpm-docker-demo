# fpm-docker-demo

Build packages using a [https://github.com/jordansissel/fpm/wiki](fpm) via docker

- Running

```
$ sudo ./tasks/package/run.sh
```

- takes the files from  **install_dir/** and creates

```
$ tasks/package/artifacts/fpm-demo-server-plugins-X_Y_all.deb
$ tasks/package/artifacts/fpm-demo-client-plugins-X_Y_all.deb
```

where 

```
X = numbers of commits in this repo
Y = git commit id 
```

e.g. 

```
$ tasks/packages/artifacts/fpm-demo-client-plugins_6_924c482_all.deb 
$ tasks/packages/artifacts/fpm-demo-server-plugins_6_924c482_all.deb 
```

- Both the debs also callout the dependenices present in 

```
$ dependencies/server/deps.txt
$ dependencies/client/deps.txt
```

and mark them as dependencies in the debians created
