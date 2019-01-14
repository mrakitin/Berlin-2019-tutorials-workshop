## Plan for Sirepo tutorial 01/16/2019

### 1. Overview of Sirepo:
  - Calculation of parameters of synchrotron radiation (SR): Source page
  - Calculation of wavefront propagation: Beamline page
  - Types of simulations (single-electron fully coherent, multi-electron partially coherent)
  - Exporting/importing features
  - Login using GitHub authentication

### 2. Installation using Docker:
  - `docker pull radiasoft/sirepo:beta`
  - `docker run -v $PWD:/sirepo -p 8000:8000 radiasoft/sirepo:beta`

### 3. Installation using Vagrant/VirualBox:
  - https://github.com/radiasoft/sirepo/wiki/Development

### 4. Using a public Sirepo server:
  - https://sirepo.com

### 5. Examples:
  - Calculator of SR: http://localhost:8000/light#/calculator
  - Text book examples: http://localhost:8000/light#/wavefront
  - Beamline examples: http://localhost:8000/light#/light-sources

### 6. Paying attention to features:
  - Log in using GitHub auth
  - Source page:
    - Parameters of the electron beam and undulator
    - Multi-electron spectrum flux report
    - Zoom & pan, scaling/resizing of the plots, checking parameters (peak coordinates, FWHM)
    - Export Python code and run it in a Jupyter notebook at https://jupyter.radiasoft.org
  - Beamline page:
    - Optical elements: drag & drop, parameters menu and tabs
    - Automatic obtaining of the attenuation length and the refractive index decrement from http://henke.lbl.gov/optical_constants/atten2.html and http://henke.lbl.gov/optical_constants/getdb2.html (CRL, Fiber, Sample optical elements)
    - Automatic obtaining of crystal parameters from http://x-server.gmca.aps.anl.gov/x0h.html
    - Samples simulations: http://localhost:8000/srw#/beamline/BT3m60yY
    - Export as zip
    - Export as a self-extracting simulation
    - Open as a new copy
    - Discard changes to example
    - Documentation at Wiki https://github.com/radiasoft/sirepo/wiki

### 7. External calls to Sirepo:
  - https://github.com/NSLS-II/sirepo-bluesky

### 8. JSR paper on Sirepo:
  - http://journals.iucr.org/s/issues/2018/06/00/il5006
  - Simulations from the JSR paper on Sirepo:
    - https://sirepo.com/srw#/beamline/LA5qG1J1
    - https://sirepo.com/shadow#/beamline/wsGlwMqv
