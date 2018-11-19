# dmdp.tntu.edu.ua
http://dmdp.tntu.edu.ua
- Site is buidled from master branch (could be changed in settings)!

Clone repository:
```
git clone git@github.com:Ternopil-National-Technical-University/dmdp.tntu.edu.ua.git
```
Change directory permission and cd to one:
```
chmod o+w dmdp.tntu.edu.ua/
cd dmdp.tntu.edu.ua
```

From the same folder run:
```
docker create --name dmdp.tntu.edu.ua  -v "$PWD":/srv/jekyll -w /srv/jekyll -p 4000:4000  -e LC_ALL=C.UTF-8 jekyll/builder /bin/bash -c 'jekyll serve'

```
Than run

```
docker start dmdp.tntu.edu.ua
```

check logs of running container:

```
docker logs dmdp.tntu.edu.ua
```
