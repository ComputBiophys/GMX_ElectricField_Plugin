This is a gromacs plugin made to add an extra input for constant electric field in .mdp file.
Current gromacs (up to gromacs-2023) only support one electric field input in each dimension (x, y, z). However, it is necessary to add two electric field components in one dimension simultaniously, eg. adding a constant transmembrane potential and a oscillating field. Currently, this can only be done by building a double-layer system to produce the transmembrane potential, which definately increases computational cost.
Here, an easy and direct solution is provided, as an extra input for constant electric field is added. To use this, simply add

constant-electric-field-x = Ex
constant-electric-field-y = Ey
constant-electric-field-z = Ez

to your .mdp file, where Ex, Ey, Ez are the electric fields to add in that dimension in V/nm.

This plugin needs to be added to gromacs source file folder before compiling. Run INSTALL to include this into the source code, and then compile gromacs.

Thanks for your use!

Author for this plugin: Zigang Song (affiliation: School of Life Sciences, Peking University)
For any questions or feedback, please connect <songzigang@stu.pku.edu.cn>.

