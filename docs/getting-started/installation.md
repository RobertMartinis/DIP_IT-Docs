# Installation

DIP_IT comes with its own installer. To install the application, run `DIP_IT_Installer.exe` and follow the installation steps.

!!! note
    This application requires the MATLAB 2025a Runtime to be installed. If you do not already have it installed, the runtime can be installed through the DIP_IT installer.

## R package for Untargeted adduct detection

Untargeted adduct detection uses the R package `InterpretMSSpectrum`. To use this feature, R must be installed on your computer. It's not mandatory to install this package if you want to use the other features provided in this application, it's only used for the untargeted adduct detection.

### Install R

Download and install R from:

https://cran.r-project.org/

After installation, make sure R is available from the system command line. On Windows, this may require adding the R installation folder to your system `PATH`.

Typical R paths on Windows look like:

```text
C:\Program Files\R\R-4.x.x\bin
C:\Program Files\R\R-4.x.x\bin\x64
```

To check whether R is available, open Command Prompt or PowerShell and run:

```bash
R --version
```

If this prints the installed R version, R is available on your path.

### Install InterpretMSSpectrum

Open R or RStudio and install the package:

```r
install.packages("InterpretMSSpectrum")
```

After installation, test that the package loads correctly:

```r
library(InterpretMSSpectrum)
```

If the package loads without errors, untargeted adduct detection should be available in DIP_IT.

### Java Runtime

Some R package functionality and supporting tools may require Java. If you encounter Java-related errors, install a Java Runtime Environment.

You can install a current Java runtime from one of these sources:

* [Eclipse Temurin](https://adoptium.net/)
* [Oracle Java](https://www.oracle.com/java/technologies/downloads/)

After installation, restart MATLAB or the DIP_IT application so the updated system environment is detected.

To check Java from the command line, run:

```bash
java -version
```

If Java is installed correctly, this prints the installed Java version.

## Troubleshooting

### R is installed but DIP_IT cannot find it

Make sure the R `bin` folder is added to the Windows `PATH`, then restart DIP_IT.

You can verify this by running the following command from a new terminal window:

```bash
R --version
```

### InterpretMSSpectrum is installed but adduct detection fails

Open R and check:

```r
library(InterpretMSSpectrum)
```

If this fails, reinstall the package and check that all package dependencies installed correctly.

### Java-related errors

If R or `InterpretMSSpectrum` reports Java-related errors, install Java and restart DIP_IT. On some systems, you may also need to restart Windows after installing Java.
