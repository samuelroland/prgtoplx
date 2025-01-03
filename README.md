# mdtoplx
### Migration tool to migrate PRG1 and PRG2 Markdown exos to PLX TOML files

**STATUS**: very drafty and not usable for now...

## Quick try
```sh
cargo install --git https://github.com/samuelroland/mdtoplx
mdtoplx # it will clone PRG1 repository for the demo and start parsing and compilation
```

## TODOs
- [x] Basic exo parsing (title, instructions, expected output, solution code)
- [ ] Refactor project in modules, add parsing tests
- [ ] Support of extracting full instruction in Markdown (not just Text node joined with \n)
- [ ] Support of multiple solutions files
- [ ] Support wrapping code inside a default main ?
- [ ] Support automatic code formatting with given `.clang-format`
- [ ] Support quick fixes like adding missing imports suggested in error outputs
    ```sh
    target/main.c:1:1: note: ‘FILE’ is defined in header ‘<stdio.h>’; this is probably fixable by adding ‘#include <stdio.h>’
    +++ |+#include <stdio.h>
    ```
- [ ] Generate default check with basic output validation
- [ ] Validate all solution files can be compiled
- [ ] Implement a filter list
- [ ] Implement a way to not erase modifications
- [ ] Generate `exo.toml` with parsed exo
- [ ] Generate `skill.toml` and `course.toml` associated with parsed exos
- [ ] 

## Goal
- [ ] Migrate programming exos in [PRG1 bucket](https://github.com/PRG1-HEIGVD/PRG1_Recueil_Exercices)
- [ ] Migrate programming exos in [PRG2 bucket](https://github.com/PRG2-HEIGVD/PRG2_Recueil_Exercices)

## Future goals
- [ ] Migrate programming exos in ASD bucket ?
- [ ] Migrate programming exos in PCO bucket ?

