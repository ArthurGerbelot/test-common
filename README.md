# How to use it as submodule

On the other app:

```
mkdir modules
cd modules
git submodule add https://github.com/ArthurGerbelot/test-common.git
cd ..
yarn add file:modules/test-common
```

# How to update 

On this repository:
```
yarn dist 
git add . 
git commit -m "Commit Message"
git push
```

On the other app:
```
git submodule update --remote 
yarn upgrade @test/common
```
