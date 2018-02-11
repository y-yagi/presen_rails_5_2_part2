#### [Recyclable cache keys](https://github.com/rails/rails/pull/29092)

```
# before
views/users/index:6e20170b482b34f88f6398ebcfa817c5/users/2-20170518223821145914
^template path    ^template tree digest            ^class ^id ^version

# after
views/users/index:6e20170b482b34f88f6398ebcfa817c5/users/2
^template path    ^template tree digest            ^class ^id
```

* version情報はcacheの中に含まれるので、cache取得後、versionが違えばcacheが更新されるようになった
* cacheのkey変わるので気をつけてね!
