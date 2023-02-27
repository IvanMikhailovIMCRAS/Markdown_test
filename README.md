# Markdown_test
For my own trainings with Markdown into Github

## PEPs list
```
https://peps.python.org/pep-0000/
```

## Guide to python ecosystem

```
https://gcoder.ru/delaem-vse-pravilno-proekt-na-python-v-2021/
```

## module typing for annotations
```
https://proglib.io/p/annotacii-tipov-v-python-vse-chto-nuzhno-znat-za-5-minut-2022-01-30
https://habr.com/ru/company/lamoda/blog/432656/
```
## How to install python3.9

```console
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.9
```
test:
```console
python3.9 --version
```

## How to install pyenv
See link 
```
https://ubunlog.com/ru/pyenv-instala-multiples-versiones-de-python-en-tu-sistema/
```
or do follow
```console
rm -fr ~/.pyenv
sudo apt-get install -y make build-essential git libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev xz-utils tk-dev
curl -L https://raw.githubusercontent.com/pyenv/pyenv-installer/master/bin/pyenv-installer | bash
```
and add to ```~/.bash_profile``` next strings:
```bash
export PATH="/home/USER/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```
then activate it:
```
source ~/.bash_profile
```
test:
```console
pyenv install –list
```

## tree

```shell
project
│   README.md
│   file001.txt    
│
└───folder1
│   │   file011.txt
│   │   file012.txt
│   │
│   └───subfolder1
│       │   file111.txt
│       │   file112.txt
│       │   ...
│   
└───folder2
    │   file021.txt
    │   file022.txt
```

## code highlighting

```python
import numpy

X = np.uniform(0,1,100)
```


```fortran
program test
implicit none
real(8) :: x(3)
integer(4), allocateable, dimension(:,:) :: mat
integer i, j, n, m

n = 3
m = 4
allocate(mat(1:n,1:m))
do i = 1, n
  do j = 1, m
    mat(i,j) = dble(i) + dble(j)
  enddo
enddo
deallocate(mat)

end program test
```
