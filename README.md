# Particle Swarm Optimization (PSO)

### Description  
Implementation of **Particle Swarm Optimization (PSO)** in Python for the course *Fuzzy Systems and Evolutionary Computing (2024/2025)*. The project is compatible with the **softpy** library and includes two main classes:  
- `ParticleCandidate` → represents particles with position, velocity, and update methods  
- `ParticleSwarmOptimizer` → manages the population, evaluates fitness, and updates solutions iteratively  

The code is designed to be modular, extensible, and easy to adapt for different optimization problems.  

---

### Features  
- Python 3+ implementation  
- Compatible with **softpy** interface  
- Modular class design (`ParticleCandidate`, `ParticleSwarmOptimizer`)  
- Customizable parameters (population size, inertia weights, neighbors, fitness function)  
- Extensible for experimentation and hybrid approaches  

---

### Requirements  
- Python 3.x  
- Numpy  
- softpy (provided in the course)  

Install dependencies with:  
```bash
pip install numpy
```  

---

### Usage  
Clone the repository and run the Jupyter notebook or Python scripts:  
```bash
git clone https://github.com/your-username/particle-swarm-optimization.git
cd particle-swarm-optimization
```

Run with your preferred fitness function by adapting the provided examples.  

---

### Example  
```python
optimizer = ParticleSwarmOptimizer(
    fitness_func=my_fitness,
    pop_size=30,
    n_neighbors=5,
    size=10,
    lower=np.zeros(10),
    upper=np.ones(10)
)
optimizer.fit(n_iters=100)
print("Best solution:", optimizer.global_best.candidate)
print("Best fitness:", optimizer.global_fitness_best)
```  

---

### License  
This project is for educational purposes (course project, University of Pavia, University of Milan "La Statale" and University of Milano-Bicocca).  
