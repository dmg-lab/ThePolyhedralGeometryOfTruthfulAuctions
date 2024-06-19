# The polyhedral geometry of truthful auctions

This is a data supplement to an [article](https://dl.acm.org/doi/10.1007/978-3-031-32726-1_17) with the same name by [Michael Joswig](https://page.math.tu-berlin.de/~joswig/), [Max Klimm](https://www3.math.tu-berlin.de/disco/team/klimm/) and Sylvain Spitz.

Here we provide the input for computations with [TOPCOM](https://www.wm.uni-bayreuth.de/de/team/rambau_joerg/TOPCOM/index.html) or [mptopcom](https://polymake.org/mptopcom); these can be used interchangeably.
The output data is stored on [Zenodo](https://zenodo.org/records/12090597).

## Table 1: Triangulations of m-cubes

Table 1 in that article lists the numbers of orbits of triangulations of cubes with respect to various group actions.
The first two columns recall known facts; see our article for the references.
The first row refers to the case m=2, which is trivial to compute.

This data set provides the data for m=3 and m=4 with the groups Sm (stabilizer of the origin) and Gm (full group of affine automorphisms).

With mptopcom suitably installed the command for producing the output of the last two columns/last two roes of Table 1 read:
```
for dat in cube3_S3 cube3_G3 cube4_S4 cube4_G4 ; do mpirun mptopcom  --flip-cache 20000 --orbit-cache 20000 --regular < $dat.dat > $dat.out ; done
```

## Table 2: Triangulations of $(\Delta_{n-1})^m$

The relevant files for Table 2 are (in the order they appear in the table):

cube3.dat, cube3_S2xS2xS2.dat, cube3_S2xS3.dat
cube4.dat, cube4_S2xS2xS2xS2.dat, cube4_S2xS4.dat
D2xD2.dat, D2xD2_S3xS3.dat, D2xD2_S3xS2.dat
D3xD3.dat, D3xD3_S4xS2.dat, D3xD3_S4xS4.dat
