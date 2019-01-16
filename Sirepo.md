# https://github.com/mrakitin/Berlin-2019-tutorials

## Plan for Sirepo tutorial 01/16/2019

### 1. Installation using Docker (~5 minutes):
  - `docker pull radiasoft/sirepo:beta`
  - `docker run -v $PWD:/sirepo -p 8000:8000 radiasoft/sirepo:beta`
  - access it at http://localhost:8000

### 2. Installation using Vagrant/VirualBox (~20 minutes):
  - https://github.com/radiasoft/sirepo/wiki/Development
  - access it at http://10.10.10.10:8000

### 3. Using a public Sirepo server:
  - https://sirepo.com

### 4. Overview of Sirepo:
  - Browser of simulations
  - Calculation of parameters of synchrotron radiation (SR): Source page
  - Calculation of wavefront propagation: Beamline page
  - Types of simulations (single-electron fully coherent, multi-electron partially coherent)
  - Exporting/importing features

### 5. Examples:
  - Calculator of SR: https://sirepo.com/light#/calculator
  - Text book examples: https://sirepo.com/light#/wavefront
  - Beamline examples: https://sirepo.com/light#/light-sources

### 6. Paying attention to features:
  - Log in using GitHub authentication (for https://sirepo.com only)
  - Source page:
    - Parameters of the electron beam and undulator (idealized and tabulated)
    - Multi-electron spectrum flux report
    - Zoom & pan, scaling/resizing of the plots, checking parameters (peak coordinates, FWHM)
    - Export Python code and run it in a Jupyter notebook at https://jupyter.radiasoft.org
  - Beamline page:
    - Optical elements: drag & drop, parameters menu and tabs
    - Propagation parameters
    - Height profiles of optical elements
    - Partially-coherent simulations
    - Automatic obtaining of the attenuation length and the refractive index decrement from http://henke.lbl.gov/optical_constants/atten2.html and http://henke.lbl.gov/optical_constants/getdb2.html (CRL, Fiber, Sample optical elements)
    - Automatic obtaining of crystal parameters from http://x-server.gmca.aps.anl.gov/x0h.html
    - Samples simulations: https://sirepo.com/srw#/simulations -> Examples -> "Sample from Image"
  - List of simulations:
    - Export as zip
    - Export as a self-extracting simulation
    - Open as a new copy
    - Discard changes to example
  - Documentation:
    - Wiki https://github.com/radiasoft/sirepo/wiki

### 7. JSR paper on Sirepo:
  - http://journals.iucr.org/s/issues/2018/06/00/il5006
  - Simulations from the JSR paper on Sirepo:
    - https://sirepo.com/srw#/beamline/LA5qG1J1
    - https://sirepo.com/shadow#/beamline/wsGlwMqv

### 8. External calls to Sirepo (please come to the next tutorial for the demo):
  - https://github.com/NSLS-II/sirepo-bluesky
