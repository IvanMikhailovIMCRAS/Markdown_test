# Markdown_test
For my own trenings with Markdown into Github

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
