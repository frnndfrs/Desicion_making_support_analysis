<div align = "center"> 
   
# Desicion making  support analysis - Instituto Tecnológico y de Estudios Superiores de Monterrey
<div align = "left"> 

# Collaborative activity: Mini case 1 - Linear programming - Group 351
- María Fernanda Frías Carranza 
- Ana Sofía Ordaz Infansón	
- Sarahí Gómez Montiel	
- Ricardo Yael Carmona Zilli	 
- Jeniffer López Vilchis	
# Question set

Consider the WhiskasModel1.py

#### 1. What are the two parameters that the LpProblem function implements?
“Chicken percent” and “Beef percent”

#### 2. Is it mandatory to name thr prob variable as prob?
Is not mandatory to the the variable as prob, since a variable is a set of characters that can be assigned a value, you can assign any name to this variable. However, it is advisable to assign it a recognizable name that is associated with the format.

#### 3. What are LpContinous and LpInteger used for?
LpContinuous refers to continuous variables, any real value, integer and fractional values are considered, on the other hand LpInteger is for integer values, discrete numbers, without decimal values, where the answer has no fractional values. 

#### 4. Explain and copy the section of code that defines the objective function.
$The$ $objective$ $function$ $is$ $added$ $to$ $'prob'$ $first$

prob += 0.013 * x1 + 0.008 * x2, "Total Cost of Ingredients per can"

#### 5. Explain and copy the section of code that defines the constraints.
$The$ $five$ $constraints$ $are$ $entered$ 

prob += x1 + x2 == 100, "PercentagesSum"
   
prob += 0.100 * x1 + 0.200 * x2 >= 8.0, "ProteinRequirement"
   
prob += 0.080 * x1 + 0.100 * x2 >= 6.0, "FatRequirement"
   
prob += 0.001 * x1 + 0.005 * x2 <= 2.0, "FibreRequirement"
                                      
prob += 0.002 * x1 + 0.005 * x2 <= 0.4, "SaltRequirement"

#### 6. Is this a minimization or maximization problem?
Minimization

#### 7. Run the WhiskasModel1.py code. (no need to make changes, just runt it as is) What is the value of the following variables.
- Status:
   BeefPercent = 66.67%
   ChickenPercent = 33.33%
   Total Cost of Ingredients per can = .96 cents per can
 - Status Full Formulation:
   BeefPercent = 60%
   ChickenPercent = 40%
   Total Cost of Ingredients per can = .52 cents per can
