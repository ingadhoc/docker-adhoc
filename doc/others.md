# Odoo optimization notes

## Numpy

OpenBLAS creates a number of threads equal to the number of core threads available so it quickly reached limit_memory_hard and the process was killed (SIGSEGV)

[+info](https://odoo-community.org/groups/contributors-15/contributors-186006?mode=thread&date_begin=&date_end=)

```env
OPENBLAS_NUM_THREADS=1
```
