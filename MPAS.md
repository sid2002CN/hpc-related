# 1.Prerequisites

## 1.C and Fortran compilers

Check Commands:

```
gcc --version
gfortran --version
```



## 2.I/O libraries

### NetCDF:

#### Requirements:

##### zlib:

Source code:

[zlib Home Site](http://www.zlib.net/)

```
$ # Build and install zlib
$ ZDIR=/home/${netid}/dirtothebuild
$ ./configure --prefix=${ZDIR}
$ make check
$ make install
```



##### hdf5:

Source code:

[HDF5® Source Code - The HDF Group](https://www.hdfgroup.org/downloads/hdf5/source-code/)

```
$ # Build and install HDF5
$ H5DIR=/home/${netid}/dirtothebuild
$ ./configure --with-zlib=${ZDIR} --prefix=${H5DIR} --enable-hl --enable-parallel
$ make check
$ make install
```



#### Source Code:

[NetCDF](https://github.com/Unidata/netcdf-c/releases?page=3)

Version needed: 4.4.x

#### Documentation:

[NetCDF Users Guide: Getting and Building netCDF (ucar.edu)](https://docs.unidata.ucar.edu/nug/current/getting_and_building_netcdf.html#getting)



### PnetCDF:

#### Requirements:

MPI C compiler: To be done

#### Source Code:

[Parallel-netcdf](https://trac.mcs.anl.gov/projects/parallel-netcdf/wiki/Download)

Version needed: 1.8.x

#### Documentation:

[PnetCDF/INSTALL at master · Parallel-NetCDF/PnetCDF · GitHub](https://github.com/Parallel-NetCDF/PnetCDF/blob/master/INSTALL)



### PIO:

[PIO](https://github.com/NCAR/ParallelIO/releases)

Version needed: 1.7.1 or 1.9.23



### Useful commands:

Unzip:

```
tar -xvf filename.tar.gz
```

