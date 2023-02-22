# G'MIC
Command-line tools for rapidly processing image-based data on Linux systems using [G'MIC](https://gmic.eu).
Includes a variety of useful operations including highly parallel maximum intensity projections, segmentation, smoothing, and more. Intially assembled by [Dr. Philippe Roudot](https://centuri-livingsystems.org/p-roudot/) for operation on [BioHPC](https://portal.biohpc.swmed.edu/content/), the high-performance computing facility at UT Southwestern Medical Center. Originally developed by [Jérôme Boulanger](https://github.com/jboulanger/jboulanger-gmic/blob/master/jboulanger.gmic).

### Requirements[^1]
- [G'MIC](https://gmic.eu) - Tested on version 2.1.1
- [GNU Parallel](https://www.gnu.org/software/parallel/) - Tested on version 20150122.


### Installation Directions
- Clone the GMIC repository.
- Navigate to the cloned repository
- Right-click on `installQuickMIPDisp.sh`, select properties, and under permissions allow executing the file as a program.
- Open a terminal, and drag and drop `installQuickMIPDisp.sh' to the terminal and hit enter[^2].
- The command  will be available on every newly opened terminal window[^3}.

### Example Operation
```
quickMIPMontage /path/to/your/3D/images
```

### Example Operation

[^1]: If you are operating this software on BioHPC, these dependencies are already installed.
[^2]: If you open the file `installQuickMIPDisp.sh` you can see what Linux commands it is executing. Summarized briefly, the shell script is reating a directory called `gmic-scripts-install` in your HOME directory, copying the necessary files to this directory and changing their permissions to allow executing these files as program, and adding these files to your Linux PATH so that you can call them from a terminal.
[^3]: When you update your Linux PATH, you will need to restart your terminal session in order for the changes to take place.
