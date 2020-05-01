FROM python:3.7

RUN apt-get update && apt-get install -y libsuitesparse-dev gmsh wget tar

RUN wget http://gmsh.info/bin/Linux/gmsh-4.5.2-Linux64.tgz
RUN tar zvxf gmsh-4.5.2-Linux64.tgz
RUN cp gmsh-4.5.2-Linux64/bin/gmsh /usr/bin

RUN pip install numpy\
    scipy\
    matplotlib\
    ipython\
    meshio\
    dmsh\
    pacopy\
    pygmsh\
    pyamg\
    pytest\
    jupyter

RUN pip install scikit-sparse

CMD /bin/bash