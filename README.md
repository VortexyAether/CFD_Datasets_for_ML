# CFD Datasets for Machine Learning

A curated collection of Computational Fluid Dynamics (CFD) datasets for machine learning-based surrogate modeling and scientific machine learning applications.

## Table of Contents
- [Aerodynamics Datasets](#aerodynamics-datasets)
- [Turbulence Datasets](#turbulence-datasets)
- [Multiphase Flow Datasets](#multiphase-flow-datasets)
- [Heat Transfer Datasets](#heat-transfer-datasets)
- [General CFD Datasets](#general-cfd-datasets)
- [Benchmark Datasets](#benchmark-datasets)
- [Contributing](#contributing)

---

## Aerodynamics Datasets

### AirfRANS: High Fidelity Computational Fluid Dynamics Dataset
- **Paper**: [AirfRANS: High Fidelity Computational Fluid Dynamics Dataset for Approximating Reynolds-Averaged Navier-Stokes Solutions](https://arxiv.org/abs/2212.07564)
- **Dataset Link**: [Hugging Face Dataset](https://huggingface.co/datasets/AirfRANS/AirfRANS)
- **GitHub**: [https://github.com/Extrality/AirfRANS](https://github.com/Extrality/AirfRANS)
- **Description**: Large-scale dataset containing RANS simulations of 2D airfoils with various shapes and flow conditions
- **Size**: ~1000 simulations with different geometries and flow parameters
- **Format**: HDF5
- **Application**: Airfoil aerodynamics, surrogate modeling, flow prediction

### ShapeNet-Airfoils
- **Paper**: [Learning to Optimize Aerodynamic Shapes](https://arxiv.org/abs/2202.09301)
- **Dataset Link**: Contact authors or check paper supplementary materials
- **Description**: Dataset of airfoil shapes with corresponding aerodynamic coefficients
- **Application**: Shape optimization, inverse design

### NACA Airfoil Database
- **GitHub**: [https://github.com/daptablade/naca-airfoil-database](https://github.com/daptablade/naca-airfoil-database)
- **Description**: Collection of NACA airfoil coordinates and simulation results
- **Format**: CSV, JSON
- **Application**: Airfoil analysis, machine learning training data

---

## Turbulence Datasets

### Johns Hopkins Turbulence Database (JHTDB)
- **Website**: [http://turbulence.pha.jhu.edu/](http://turbulence.pha.jhu.edu/)
- **Paper**: [A Public Turbulence Database Cluster and Applications to Study Lagrangian Evolution of Velocity Increments in Turbulence](https://arxiv.org/abs/0804.1703)
- **Description**: Large-scale direct numerical simulation (DNS) data for isotropic turbulence, channel flow, and other canonical flows
- **Size**: Multi-terabyte datasets
- **Format**: Custom access through web services API
- **Application**: Turbulence modeling, flow statistics, ML for turbulence

### Turbulent Channel Flow DNS
- **GitHub**: [https://github.com/turbulent-channel-flow](https://github.com/turbulent-channel-flow)
- **Description**: Direct numerical simulation data for turbulent channel flows at various Reynolds numbers
- **Application**: Wall-bounded turbulence, RANS/LES model development

### KTH FLOW Turbulence Database
- **Website**: [https://www.flow.kth.se/](https://www.flow.kth.se/)
- **Description**: Various turbulence simulation datasets from KTH Royal Institute of Technology
- **Application**: Turbulence research, validation datasets

---

## Multiphase Flow Datasets

### Two-Phase Flow Dataset
- **Paper**: [Machine Learning for Two-Phase Flow](https://arxiv.org/abs/2106.12656)
- **Description**: Simulations of two-phase flows with various void fractions and flow regimes
- **Application**: Multiphase flow prediction, regime classification

### Bubble Column Datasets
- **GitHub**: [https://github.com/multiphaseflow/bubble-columns](https://github.com/multiphaseflow/bubble-columns)
- **Description**: Experimental and simulation data for bubble column reactors
- **Application**: Bubbly flow modeling, reactor design

---

## Heat Transfer Datasets

### Conjugate Heat Transfer Dataset
- **Description**: Datasets for conjugate heat transfer problems coupling fluid flow and heat conduction
- **Application**: Thermal management, heat exchanger design

### Natural Convection Benchmarks
- **Paper**: Various benchmark papers from ASME and other organizations
- **Description**: Standard benchmark cases for natural convection (e.g., differentially heated cavity)
- **Application**: Model validation, heat transfer prediction

---

## General CFD Datasets

### Cylinder Flow Dataset (Re=100-1000)
- **GitHub**: [https://github.com/cfd-ml/cylinder-flow](https://github.com/cfd-ml/cylinder-flow)
- **Description**: Flow past circular cylinder at various Reynolds numbers
- **Format**: VTK, NumPy arrays
- **Application**: Vortex shedding prediction, reduced-order modeling

### Cavity Flow Datasets
- **Description**: Lid-driven cavity and other cavity flow configurations
- **Application**: Benchmark testing, flow pattern learning

### OpenFOAM Tutorial Cases
- **GitHub**: [https://github.com/OpenFOAM/OpenFOAM-dev/tree/master/tutorials](https://github.com/OpenFOAM/OpenFOAM-dev/tree/master/tutorials)
- **Description**: Comprehensive collection of tutorial cases covering various CFD applications
- **Format**: OpenFOAM native format
- **Application**: Learning, validation, diverse CFD scenarios

---

## Benchmark Datasets

### PDEBench: Benchmark Datasets for Data-Driven PDE Solvers
- **Paper**: [PDEBench: An Extensive Benchmark for Scientific Machine Learning](https://arxiv.org/abs/2210.07182)
- **GitHub**: [https://github.com/pdebench/PDEBench](https://github.com/pdebench/PDEBench)
- **Dataset Link**: [Hugging Face](https://huggingface.co/datasets/pdebench/PDEBench)
- **Description**: Large-scale benchmark with various PDE problems including fluid dynamics
- **Size**: Multiple datasets with varying complexity
- **Application**: PDE solver benchmarking, ML model comparison

### PhysX: Physics Simulation Datasets
- **Paper**: [Learning to Simulate Complex Physics with Graph Networks](https://arxiv.org/abs/2002.09405)
- **GitHub**: [https://github.com/google-deepmind/deepmind-research/tree/master/learning_to_simulate](https://github.com/google-deepmind/deepmind-research/tree/master/learning_to_simulate)
- **Description**: Particle-based fluid simulation datasets
- **Application**: Graph neural networks for physics, particle dynamics

### Navier-Stokes Datasets for Neural Operators
- **GitHub**: [https://github.com/neuraloperator/neuraloperator](https://github.com/neuraloperator/neuraloperator)
- **Dataset Link**: [Google Drive Links in Repository](https://github.com/neuraloperator/neuraloperator)
- **Description**: Various 2D and 3D Navier-Stokes simulations for neural operator training
- **Application**: Neural operators, surrogate modeling

### Physics-Informed Neural Networks (PINN) Datasets
- **GitHub**: [https://github.com/maziarraissi/PINNs](https://github.com/maziarraissi/PINNs)
- **Description**: Various fluid dynamics problems for PINN training and testing
- **Application**: Physics-informed machine learning

---

## Contributing

We welcome contributions to expand this collection! To add a new dataset:

1. **Fork this repository**
2. **Add your dataset** following the format:
   ```
   ### Dataset Name
   - **Paper**: [Title](link) (if applicable)
   - **Dataset Link**: Direct link to dataset
   - **GitHub**: Repository link (if applicable)
   - **Description**: Brief description of the dataset
   - **Size**: Dataset size (if known)
   - **Format**: Data format (e.g., HDF5, VTK, CSV)
   - **Application**: Primary use cases
   ```
3. **Submit a pull request** with a clear description

### Guidelines for Contributions
- Ensure the dataset is publicly accessible or provide clear access instructions
- Include proper citations for academic datasets
- Verify all links are working
- Add datasets to the appropriate category or create a new category if needed

---

## License

This repository is a collection of links and references. Please refer to individual datasets for their specific licenses and terms of use.

## Citation

If you use datasets from this collection in your research, please cite the original papers and acknowledge the dataset creators.

---

**Maintained by**: CFD-ML Community  
**Last Updated**: October 2025

For questions or suggestions, please open an issue on GitHub.
