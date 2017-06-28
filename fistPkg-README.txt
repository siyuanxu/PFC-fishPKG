;fname: fistPkg-README.txt

Material-modeling support for PFC 5.0 is provided in the PFC 5.0 FISHTank (or
fistPkg). We describe the fistPkg as the material-modeling support package.

CAPABILITIES
  Material genesis of linear, contact-bonded, parallel-bonded, flat-jointed
  and user-defined (3D hill) materials in polyaxial, cylindrical and spherical
  vessels. Material grains can be either balls or clumps. Material tests are
  compression (confined, unconfined and uniaxial strain),
  diametral-compression and direct-tension. Microstructural monitoring
  includes properties (such as grain-size distribution) with microstructural
  plots and crack monitoring for bonded materials.

LAYOUT OF THE PFC 5.0 FISHTANK
  The PFC 5.0 FISHTank is provided as a single directory, named fistPkgN,
  where N is the version number of the PFC 5.0 FISHTank. The version number is
  also given in the file fistSrc\fistPkg-version.txt. The public-modifications
  list for the PFC 5.0 FISHTank is in the file fistPkg-publicMods.txt.
  Documentation is in the Documentation directory. Example projects are in the
  ExampleProjects directory, which also contains the FISH source code in the
  fistSrc directory.

EXAMPLE PROJECTS
  There is a MatGen example project for each material type, and these
  projects are in directories: ExampleProjects\MatGen-X, where X = {Linear,
  ContactBonded, ParallelBonded, FlatJointed, Hill}. To run example-project X,
  copy the directories fistSrc and MatGen-X to a working location (perhaps
  call it myRUNS). You can now open the 2D or 3D MatGen-X project, and after
  the run completes, you can open its XTest projects, where X = {Comp,
  DiamComp, Ten}.

DOCUMENTATION (see dirContents.txt)

INSTALLATION NOTES
  The User-Defined Material Example uses the hill contact model DLL, which
  requires the DLL file contactmodelmechanical3dhill005_64.dll to be copied
  from ExampleProjects\fistSrc to
  PFC500\exe64\plugins\contactmodelmechanical3D, where PFC500 is the PFC 5.0
  installation location.

;EOF: fistPkg-README.txt