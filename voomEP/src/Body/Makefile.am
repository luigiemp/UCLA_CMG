## Makefile.am -- Process this file with automake to produce Makefile.in
INCLUDES     =  -I$(srcdir)/../			     \
		-I$(srcdir)/../Mesh		     \
                -I$(srcdir)/../Shape/                \
                -I$(srcdir)/../VoomMath/             \
                -I$(srcdir)/../Quadrature/           \
		-I$(srcdir)/../IonicModel/           \
		-I$(srcdir)/../Material/	     \
                -I$(blitz_includes)                     \
                -I$(tvmet_includes)                     \
                -I/u/local/apps/trilinos/current/include
AM_LDFLAGS    = -L$(blitz_libraries)                    \
	        -L../	                                \
	        -L../Quadrature/ -L../IonicModel        \
	        -L../Shape/    -L../Mesh/               \
	        -L../VoomMath/                          \
	        -L/u/local/apps/mumps/4.9.2/lib         \
	        -L/u/local/apps/trilinos/current/lib     \
	        -L/u/local/apps/scalapack/current               \
	        -L/u/local/apps/superlu_dist/2.4/lib            \
	        -L/u/local/apps/parmetis/3.1.1                  \
	        -L/u/local/compilers/intel/current/current/mkl/lib/em64t
LDADD         = -lblitz -lIonicModel                                   \
	        -lQuadrature                                    \
	        -lShape                                         \
	        -lVoomMath -lMesh -lMaterial

lib_LIBRARIES=libCardiacBody.a
libCardiacBody_a_SOURCES = CardiacBody.cc

