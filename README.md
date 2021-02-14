![](https://github.com/senselogic/CHYLE/blob/master/LOGO/chyle.png)

# Chyle

Style sheet usage checker.

## Installation

Install the [DMD 2 compiler](https://dlang.org/download.html) (using the MinGW setup option on Windows).

Build the executable with the following command line :

```bash
dmd -m64 chyle.d
```

## Command line

```
chyle [options]
```

### Options

```
--include <file filter> : include matching files
--exclude <file filter> : exclude matching files
--ignore <class> : ignore this class
--unused : find unused classes
--missing : find missing classes
--verbose : show the processing messages
```

### Example

```bash
chyle --include "CSS/*.css" --include "PHP//*.php" --unused --missing --verbose
```

List unused and missing classes in the matching CSS and PHP files.

## Version

1.0

## Author

Eric Pelzer (ecstatic.coder@gmail.com).

## License

This project is licensed under the GNU General Public License version 3.

See the [LICENSE.md](LICENSE.md) file for details.
