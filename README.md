# repo
sunshinesong's repo.

### tip myself

#将位于debs目录的所有deb包扫描并生成Packages
dpkg-scanpackages -m debs/ > Packages
#生成客户端可能需要的gz和bz2压缩的Packages
gzip -c Packages > Packages.gz
bzip2 -k Packages
