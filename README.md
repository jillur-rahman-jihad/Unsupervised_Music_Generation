# Unsupervised Music Generation Project

This project explores various approaches to music generation, including baseline methods, deep learning models with different architectures, and reinforcement learning techniques.

## Main Notebooks
- Task1_TASK3_TASK4_BASELINE_22301723.ipynb - Contains All codes of Task 1, 3, and 4
- TASK2_22301723.ipynb Contains All codes of TASK 2 (Because it was multi genre  I had to create a separate dataset and work on it separately using lakh midi)
## Midi files
- Task 1 - https://drive.google.com/drive/folders/1imN0qWL604Xqsoo7__eHUI2tN_TCq9iL?usp=sharing
- Task 2 - https://drive.google.com/drive/folders/1YcTOAg6WoDEUoyL0Svl0mn3P_kCqKRCx?usp=sharing
- Task 3 - https://drive.google.com/drive/folders/1NjlfLEP2xDVD5RmiV6i8iQOpdQMKGOiv?usp=sharing
- Task 4 - https://drive.google.com/drive/folders/1e-gaglL_lj62OLnqAeiolj5Wtl4ADqHE?usp=sharing
- Random - https://drive.google.com/drive/folders/1N_6MwY8MYnMxUyIgjeOcqAUtAjFN12mh?usp=sharing
- Markov - https://drive.google.com/drive/folders/11ELzL7dUNwjHju0W1WnQ68UOROJMqtqI?usp=sharing 

##Report
drive link - 


The project consists of four main tasks:
- **TASK 1**: Basic music generation using neural networks
- **TASK 2**: Genre-specific music generation (Classical, Jazz, Rock)
- **TASK 3**: Multi-genre music generation with sampling
- **TASK 4**: Reinforcement Learning-based music generation with reward modeling


## The project is implemented By me (Single Member)



## Directory Structure

### Root Files
- **README.md** - Project documentation (this file)
- **Task1_TASK3_TASK4_BASELINE_22301723.ipynb** - Jupyter notebook containing baseline implementations and experiments for Tasks 1, 3, and 4
- **TASK2_22301723.ipynb** - Jupyter notebook for TASK 2 experiments

### `/Files/` - Main Project Directory

#### Baseline Methods
- **Markov/** - Markov chain-based music generation
  - Contains 5 sample MIDI files generated using Markov models
  - Files: `markov_1.mid` through `markov_5.mid`

- **Random Generator/** - Random baseline music generation
  - Contains 5 sample MIDI files generated randomly
  - Files: `random_1.mid` through `random_5.mid`

#### TASK 1 - Basic Neural Network Music Generation
- **TASK1/** - Task 1 results and model
  - `best_model.pt` - Trained PyTorch model for basic music generation
  - Sample outputs: `sample_1-2.mid`, `sample_2.mid`, `sample_3.mid`, `sample_4.mid`, `sample_5.mid` (5 generated music samples)
  - Notebook: `Task1_TASK3_TASK4_BASELINE_22301723.ipynb`

#### TASK 2 - Genre-Specific VAE Music Generation
- **TASK2/** - Genre-specific music generation using Variational Autoencoders
  - `vae_music_model.pth` - Trained VAE model supporting multiple genres
  - `genre_dataset/` - Training dataset organized by genre:
    - `classical/` - Classical music MIDI files (e.g., Bach inventions, string quartets)
    - `jazz/` - Jazz music MIDI files
    - `rock/` - Rock music MIDI files
  - Sample outputs:
    - Classical: `sample_classical_1.mid`, `sample_classical_4.mid`, `sample_classical_7.mid`
    - Jazz: `sample_jazz_0.mid`, `sample_jazz_3.mid`, `sample_jazz_6.mid`
    - Rock: `sample_rock_2.mid`, `sample_rock_5.mid`
  - Notebook: `TASK2_22301723.ipynb`

#### TASK 3 - Multi-Genre Music Generation with Sampling
- **TASK3/** - Extended music generation with improved sampling techniques
  - `best_model_t3.pt` - Best trained model for Task 3
  - `survey_results.csv` - Evaluation results from user surveys
  - Sample outputs: `t3_sample_1.mid` through `t3_sample_10.mid` (10 generated music samples)
  - Notebook: `Task1_TASK3_TASK4_BASELINE_22301723.ipynb`

#### TASK 4 - Reinforcement Learning Music Generation
- **TASK4/** - RL-based music generation with reward modeling
  - `rl_policy_best.pt` - Best trained RL policy model
  - `reward_model.pt` - Reward model for evaluating music quality
  - Sample outputs: `t4_sample_1.mid` through `t4_sample_10.mid` (10 generated music samples using RL)
  - Notebook: `Task1_TASK3_TASK4_BASELINE_22301723.ipynb`

## Quick Navigation Guide

| Information Needed | Location |
|-------------------|----------|
| Experiment code for Task 1 | `Task1_TASK3_TASK4_BASELINE_22301723.ipynb` |
| Experiment code for Task 2 | `TASK2_22301723.ipynb` |
| Training dataset | `Files/TASK2/genre_dataset/` |
| Markov baseline results | `Files/Markov/` |
| Random baseline results | `Files/Random Generator/` |
| Task 1 model & samples | `Files/TASK1/` |
| Task 2 model & samples | `Files/TASK2/` |
| Task 3 model & samples | `Files/TASK3/` |
| Task 4 model & samples | `Files/TASK4/` |
| Survey evaluation results | `Files/TASK3/survey_results.csv` |

## File Format Information

- **.ipynb** - Jupyter Notebook files containing code, experiments, and results
- **.pt** - PyTorch model files (Task 1 and 3)
- **.pth** - PyTorch model files (Task 2 and 4)
- **.mid** - MIDI files (music notation format for generation samples and datasets)
- **.csv** - CSV data files (evaluation results)

## Model Descriptions

### Baseline Models
- **Markov Chain** - Statistical model based on note transition probabilities
- **Random Generator** - Random selection of notes and durations

### Deep Learning Models
- **Task 1 Model** - Basic neural network for music generation
- **Task 2 Model (VAE)** - Variational Autoencoder for genre-specific generation
- **Task 3 Model** - Improved model with better sampling strategies
- **Task 4 RL Policy** - Reinforcement Learning policy trained with reward signal

## Generated Samples

Each task contains 5-10 generated MIDI files that demonstrate the output quality:
- **Baselines**: 5 samples each for Markov and Random approaches
- **Tasks 1-3**: 5 samples for Tasks 1 and 2, 10 samples for Task 3
- **Task 4**: 10 samples generated with RL-based policy

## How to Use This Repository

1. **Review the notebooks** - Start with the Jupyter notebooks to understand the methodology
2. **Examine the datasets** - Check `Files/TASK2/genre_dataset/` to see training data
3. **Listen to samples** - Play the MIDI files in `Files/` subdirectories to hear generation results
4. **Compare approaches** - Compare baseline results with deep learning results across tasks
5. **View evaluations** - Check `Files/TASK3/survey_results.csv` for user evaluation data

## Notes

- All models are stored as PyTorch checkpoint files (.pt and .pth)
- MIDI files can be played using any MIDI player or music notation software
- The Jupyter notebooks contain the full implementation details and training procedures
- Survey results for Task 3 provide quantitative evaluation of generation quality
