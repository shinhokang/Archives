# Mac OS X

## Get Homebrew

```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## Installing xcode-select (skip if you installed via app store)
```
$ xcode-select --install
```


## Install Java8

```
$ brew update
$ brew tap caskroom/cask
$ brew install Caskroom/cask/java
```

And Java 8 will be installed at `/Library/Java/JavaVirtualMachines/jdk1.8.xxx.jdk/`

```
$ java -version 
```


## Install Scala

```
$ brew install scala
```

## Install Spark
```
$ brew install apache-spark
```

Start spark shell
```
$ spark-shell
```
