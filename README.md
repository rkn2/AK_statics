# Static Equilibrium in Remote Alaska

[![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

"Static Equilibrium in Remote Alaska" is a comprehensive educational module focused on teaching static equilibrium and physics through a combination of theory, practical examples, and computational exercises. This module integrates physics concepts with Python programming, enabling students to solve real-world problems such as calculating the load-bearing capacity of ice and designing structures like bridges in specific environmental contexts. The presented material here serves as a public version of the broader impacts from [this National Science Foundation grant](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2121909&HistoricalAwards=false). 

## Course Content:

| Lesson | Content Summary                 | Google CoLab|
|------|---------------------------------|------|
| 1    | This lesson introduces the fundamental concepts of statics, focusing on the principles of forces in equilibrium. It provides an understanding of how to solve problems involving force vectors, both through graphical and analytical methods. The lesson emphasizes the importance of understanding the conditions for equilibrium in various physical scenarios, and it guides students in applying these principles to practical, real-world problems. | [![Unit_01](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rkn2/AK_statics/blob/main/Statics_Lesson1.ipynb) |
| 2    | The lesson covers concepts like support forces and net force, and teaches students how to apply the principles of vertical and horizontal equilibrium. It emphasizes visualizing parametric relationships and includes practical examples like evaluating the stability of a person standing on ice. | [![Unit_02](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rkn2/AK_statics/blob/main/Statics_Lesson2%20(1).ipynb) |
| 3    | This lesson introduces the concepts of torque and rotational equilibrium. This lesson teaches students how to calculate torque and understand its role in physical systems, particularly focusing on its application in various equilibrium scenarios| [![Unit_03](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rkn2/AK_statics/blob/main/Statics_Lesson3.ipynb) |
| 4    | This lesson reinforces understanding of forces and equilibrium in physics and engineering, with a focus on practical problem-solving.| [![Unit_04](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rkn2/AK_statics/blob/main/Statics_Lesson4.ipynb) |
| 5    | This lesson focuses on understanding conditions for static equilibrium in bridges, including balancing forces and torques. Students learn about internal forces like shear forces and moments that contribute to equilibrium. | [![Unit_05](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rkn2/AK_statics/blob/main/Statics_Lesson5.ipynb) |

## Statement of Need
Engineering statics is a foundational course for civil and mechanical engineering students, yet many struggle to connect abstract mathematical concepts with physical reality. Traditional teaching methods often rely on static diagrams and manual calculations, which can obscure the dynamic relationship between forces, geometry, and equilibrium.

`AK_statics` addresses this gap by providing an interactive, computational approach to learning statics. By using Python and Jupyter Notebooks (via Google Colab), students can:
- **Visualize** forces and moments in real-time.
- **Experiment** with parameters (e.g., changing loads or geometry) to see immediate effects on stability.
- **Connect** engineering principles to real-world contexts, specifically the unique challenges of infrastructure in Alaska.

This module is designed for undergraduate engineering students, educators looking for open-source active learning resources, and self-learners interested in the intersection of physics and programming.

## Installation and Dependencies
The notebooks are designed to run in **Google Colab**, which requires no local installation. However, if you wish to run them locally, you will need Python 3.9+ and the following libraries:
- `numpy`
- `matplotlib`
- `ipywidgets`
- `jupyter`

You can install these using the provided requirements file:
```bash
pip install -r requirements.txt
```

## Community Guidelines
We welcome contributions! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License
This project is dual-licensed:
- **Code**: The software code is licensed under the [MIT License](LICENSE).
- **Content**: The educational content (text, images, notebooks) is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).


The document "interacting_colab.ipynb" is a guide for teachers and students on how to interact with colab notebooks. This material was produced by Google and has been reproduced for simplicity. These resources were only curated and were not written by the authors of this work. 

## Dependencies and Installation
This project uses the Python programming language, and requires Python >= 3.9.
Units are written and available as CoLab notebooks. 

## Getting started with the material
The course "Static Equilibrium in Remote Alaska" is designed primarily for first-year high school Physics students. However, it's also accessible to a wider audience for self-study or as a resource for other instructors to adapt and build upon. We provide a summary on how to engage with the material effectively for both individual learners and educators.

### Using the material as a student for self-study
For students using the material independently for self-study, simply progress through each notebook in sequence. The most straightforward approach is to use the provided Colab links, which are set up to function immediately with all necessary packages. Should you encounter any issues, often restarting the runtime environment in Colab can resolve them.

### Using the material as an educator
Instructors can flexibly utilize the course material in their teaching. Feel free to modify and adapt any part of the content to suit your teaching needs. Sharing your experiences with using the material is greatly appreciated. The most straightforward approach is to use the provided Colab links, which are set up to function immediately with all necessary packages. Should you encounter any issues, often restarting the runtime environment in Colab can resolve them.

## Authors and their contributions
Authors are, in alphabetical order:
* Davin Holen (DH)
* Heather Randel (HR)
* Megan Muckioki (MM)
* Rebecca Napolitano (RN)
* Theresa Napolitano (TN)
* Guangqing Chi (GQ)

TN has been teaching high school physics at the Academy of Our Lady of Mercy Lauralton Hall since 1993. 
RN and TN created the physics materials. HR, MM, GQ, and DH provided social science context.
DH provided context about rural Alaska.

## Acknowledgements

This material is based upon work supported by the National Science Foundation under Grant BCS-2121909 and IIS-2123343. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.
The authors would like to acknowledge the high school students who were eager to try out the materials and Dr. Thomas Boothby who provided invaluable empirical knowledge about bridges and bridge design. 

## Contributing and raising issues

Contributions to the learning resource are welcome. Contributions can be made through creating an issue or a pull request.

### For issues
To create an issue, contributors are encouraged to follow the [GitHub quickstart guide on creating an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue).
Make sure to include the following into your issue:
* Are you using the Colab or a local install version
* Are you using it as a student or instructor
* Is the issue reporting a bug, an enhancement, or a feature request

### For pull requests
To create a pull request, contributors are encouraged to follow the [GitHub quickstart guide on creating a fork and submitting a pull request.](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)

### Telling us about how you are using the resource
If you just want to tell us how you have been using the resource just send us an email or raise an issue pointing to your work. nap@psu.edu

## License
[MIT License](https://opensource.org/license/mit/) THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE
