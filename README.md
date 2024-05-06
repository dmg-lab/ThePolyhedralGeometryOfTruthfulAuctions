These files are the inputs for the enumeration of regular triangulations using MPTOPCOM.
To execute the computations, install MPTOPCOM and use

/PATH/TO/OPENMPI/bin/mpirun /PATH/TO/MPTOPCOM/bin/mptopcom < FILE.dat > RESULT.out --regular

The names of the files indicate the polytope for which the triangulations are computed as well as the symmetries considered, separated by an underscore.
Polytopes:
cube3 resp. cube4 stand for the cube of dimension 3 resp. 4
D2xD2 resp. D3xD3 stand for the product of two simplices of dimension 2 resp. 3
Symmetries:
no underscore stands for no symmetries
G3 resp. G4 stand for the full automorphism group of the cube in dimension 3 resp. 4
Sx stands for the symmetric group on x elements

The relevant files for table 1 are (in the order they appear in the table):
cube3.dat, cube3_S3.dat, cube3_G3.dat
cube4.dat, cube4_S4.dat, cube4_G4.dat

The relvant files for table 2 are (in the order they appear in the table):
cube3.dat, cube3_S2xS2xS2.dat, cube3_S2xS3.dat
cube4.dat, cube4_S2xS2xS2xS2.dat, cube4_S2xS4.dat
D2xD2.dat, D2xD2_S3xS3.dat, D2xD2_S3xS2.dat
D3xD3.dat, D3xD3_S4xS2.dat, D3xD3_S4xS4.dat
