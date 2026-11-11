DONE Add numerical before simulation to title

DONE remove list of figures

DONE electrostriction is a  bit jargony ->change in densitydue to strong electric fields DONE nonlinear ->nonlinear DONE use 'laser' first page DONE some figures first page

~DONE Equations; need to say at some poitn that a,band c are
~DONE some diagram of a grid with a specified thing at the start with an arrow, showing what we are trying to get this to look like
DONE include that we are small structures and light in and out so we use function of spacethrough time rather than other way around DONE Equations ->Eq DONE use subeq in latex DONE boundary conditions; we use FFT for boundary conditions; weakness is it doesnt allow for light to leav; describing a behaviour of a ringessentially rather than a length of fibre.Wanna make sim domain large enough s.t. effects ofexternal return nevereffect the centre of the simulation that we are interested in. DONE FFT's bake theperidoicnature into the simulation, would ened to move it away to solve from this DONE maybe move 1.7 earlier (before current 1.3) and include a bit more context about the DONE explain half step figure better. DONE we want to go from something to another something.Doing this is essentially the same astaking the exponentials of those operations DONE on numerial grid it becomes matrices and then cna take derivitive of it. DONE  e^ne^D !=E^nD but if you chop it up and awhatnot they get super close and that is the steps basically
explain RK4 that the nonlinear parts are very mixed in.D is easy, N is not,
In better english, what we mean by solvingan interaction picturewe are doing; we only care about the end result, solve half by having the operations evolve and the other half by having the wave functtions evolve. Easy part of problem to operators, hard part left on field, has effect of reducing work to do.
when solving PDE often case that some is straight forrwarrd and some isnt. if only dispersion -> can solve as far into the future in 1 step. cant for nonlinear(unless super special case) sowe cannot solve the whole problem in one step.Part of problem aint diagonisable (matrix view of it),and so an operation with an easy and hard partcan betaken through 1.4 / 1.5 appraoches and thistakes advantage of these facts of easy and hard parts 0 interlaced in a way that makes the interaction more efficient.
Can drop 1.5 rk5 complex picture.
fields that we are changing are over time, opreations never change,time does, and we updatethe fields


# DONE ALL ABOVE HERE








modelling in physics about things taht are mega small and mega big. put straight into computer, few things happen (overflow underglorw, other thing is really ahrd to tell if behaviour is correct or not).Also scale differences really just side effects of the chosen units.rescaling correctylymakes everythign become small again or more normal.Thisis called non-dimensionalisation, but experimentalists dont like to do this.
This is in the TOML file; numbers put in and so both approaches of physical numbers and scaled numbers can both work for all types of physicists



add new physics in localised code fashion for people wanting newnon-lienar or whatever.



provide history toexisting codebase stuff, code size, libs, design choices,
Maybe mention the .setup() rather than constructors.



GPU vs CPU maybedont use thecodebase specific stuff in it.




Introductiont o the methodoogy;generally 3 parts,one was getting used to code /custom functionality,

maybe bring up modern C++ more explicity. Bring up tradeoff between polymorhipsm and std::variant


