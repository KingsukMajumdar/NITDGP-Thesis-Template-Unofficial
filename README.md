# 🎓 LaTeX Thesis Template  [Unofficial] for National Institute Of Technology Durgapur 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat&logo=latex&logoColor=white)](https://www.latex-project.org/) [![Version](https://img.shields.io/badge/Version-V1.0-blue.svg)](https://github.com/) [![Overleaf](https://img.shields.io/badge/Overleaf-47A141?style=flat&logo=overleaf&logoColor=white)](https://www.overleaf.com/) [![YouTube](https://img.shields.io/badge/YouTube-FFFFFF?style=flat&logo=YouTube&logoColor=red)](https://www.youtube.com/@LearnWithKingsuk) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white)](https://github.com/KingsukMajumdar/NITDGP-Thesis-Template-Unofficial.git)


A professional, feature-rich LaTeX template [**Unofficial**]  for undergraduate, postgraduate, and doctoral thesis at **National Institute Of Technology Durgapur**. This template provides automated formatting, multi-student support, and institutional compliance while maintaining academic presentation standards.

With Regards  
Kingsuk Majumdar, Ph.D. (Engg.)


M. Tech (EE, 2013) & Ph.D (EE, 2023)

---

## 🌟 Key Features

- 📄 **Professional A4 formatting** optimized for academic thesis
- 👥 **Multi-student support** (1-3 students for UG, 1 for PG/PhD) with automatic conditional rendering
- 🖼️ **Integrated photo handling** for author biographies with wrapfigure layout
- 🎨 **Customizable headers, footers, and title pages**
- 📝 **Justified text without hyphenation** for clean appearance
- 💻 **MATLAB code highlighting** via mcode.sty package
- 🔧 **Comprehensive error handling** and wrapper commands
- 📚 **Complete frontmatter and backmatter** templates
- 🏷️ **Short title support** for footers
- 📖 **Automatic bibliography** and abbreviations handling
- 🔄 **Degree-specific configurations** (UG/PG/PhD requirements)
- ⚡ **latexmk support** for automated compilation
- 🏫 **Flexible supervisor college** configuration

---

## 📁 Directory Structure

```
ug-thesis-template/
|-- main.tex                    # Main document file (User Input Section)
|-- thesis.cls                  # LaTeX class file (Formatting Engine)
|-- references.bib              # Bibliography database
|-- mcode.sty                   # MATLAB code highlighting package
|-- .latexmkrc                  # latexmk configuration (optional)
|-- README.md                   # Documentation file
|-- LICENSE.lic                 # License information
|-- Frontmatter/
|   |-- Declaration.tex         # Student declaration page (Don't Change it) 
|   |-- Certificate.tex         # Supervisor approval certificate (Don't Change it)
|   |-- Acknowledgment.tex      # Acknowledgments section
|   |-- Abstract.tex            # Abstract and keywords
|   +-- Acronyms.tex            # List of abbreviations and nomenclature
|-- Chapters/
|   |-- Chapter01_Introduction.tex    # Introduction chapter (MUST BE)
|   |-- Chapter02_Literature.tex      # Literature review (MUST BE)
|   |-- Chapter02_Table.tex           # Table examples
|   |-- Chapter03_Figure.tex          # Figure examples
|   |-- Chapter04_Math.tex            # Mathematical expressions
|   |-- Chapter03_Methodology.tex     # Research methodology
|   |-- Chapter04_Implementation.tex  # Implementation details
|   |-- Chapter05_Results.tex         # Results and analysis (MUST BE)
|   +-- Chapter06_Conclusion.tex      # Conclusions and future work (MUST BE)
|-- Backmatter/
|   |-- PublicationsList.tex    # Publications by authors
|   +-- AuthorBio.tex           # Author biographies (Strictly PG/PhD only)
|-- Figures/
|   |-- college_logo.png        # Institutional logo (required)
|   |-- StudentOne_photo.jpg    # Student photograph
|   |-- StudentTwo_photo.jpg    # Student photograph
|   |-- StudentThree_photo.jpg  # Student photograph
|   |-- Chapter01/              # Chapter-wise figure organization
|   |-- Chapter02/
|   |-- Chapter03/
|   |-- Chapter04/
|   |-- Chapter05/
|   +-- Chapter06/
+-- OUTPUT/                     # Generated output files (after compilation)
    |-- main.pdf                # Final thesis document
    |-- main.aux                # Auxiliary file
    |-- main.bbl                # Bibliography file
    |-- main.blg                # Bibliography log
    |-- main.log                # Compilation log
    |-- main.toc                # Table of contents
    |-- main.lof                # List of figures
    +-- main.lot                # List of tables
```

---

## 🚀 Quick Start

### 📦 Requirements

- **LaTeX Distribution**: TeX Live (Linux/Mac) or MiKTeX (Windows)
- **Compiler**: pdfLaTeX
- **OS**: Manjaro Linux (recommended) or any Linux distribution
- **Editor**: TeXstudio, VS Code, Overleaf, or any LaTeX editor
- **Optional**: latexmk for automated compilation

### 🔧 Installation (Manjaro Linux)

```bash
# Update system repositories
sudo pacman -Syu

# Install complete LaTeX distribution
sudo pacman -S texlive-most texlive-bibtexextra

# Alternative: Install full TeX Live distribution
sudo pacman -S texlive-core texlive-bin texlive-latexextra texlive-fontsextra

# Install latexmk for automated compilation
sudo pacman -S texlive-binextra
```

### 📥 Getting Started

1. **Clone the repository**
   ```bash
   git clone [GitHub repository link will be added here]
   cd ug-thesis-template
   ```

2. **Configure your thesis** (Edit `main.tex` USER INPUT SECTION)
   ```latex
   %% Thesis Information
   \ThesisTitle{Your Thesis Title Here}
   \ShortTitle{Short Title for Footer}
   \Department{Department of Electrical Engineering}
   \College{National Institute Of Technology Durgapur}
   \DegreeType{Bachelor of Technology (B. Tech.)}  % or M. Tech. or Ph.D.
   \NumberOfStudents{3}  % 1-5 for UG, 1 for PG/PhD
   
   %% Student Information
   \StudentOne{Your Name}
   \RollOne{21/EE/001}
   \RegOne{214410301001}
   \EmailOne{your.email@student.nitdgp.ac.in}
   
   %% Supervisor Information
   \Supervisor{Dr. Your Supervisor Name}
   \SupervisorDesignation{Professor}
   \SupervisorDept{Department of Electrical Engineering}
   \SupervisorCollege{National Institute Of Technology Durgapur}
   ```

3. **Add your content**
   - Edit `Frontmatter/Abstract.tex`
   - Edit `Frontmatter/Acknowledgment.tex`
   - Edit chapter files in `Chapters/` directory
   - Add references to `references.bib`

4. **Add images**
   - Place `college_logo.png` in `Figures/` directory
   - Add student photos as specified in configuration
   - Organize chapter figures in respective subdirectories

---

## ⚡ Compilation

### 🖥️ Offline Compilation (Manjaro Linux)

#### Method 1: Traditional Compilation
```bash
# Navigate to project directory
cd /path/to/ug-thesis-template/

# Create output directory
mkdir -p OUTPUT

# Primary compilation sequence
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex

# Move generated files to OUTPUT directory
mv main.pdf OUTPUT/
mv *.aux *.bbl *.blg *.log *.toc *.lof *.lot OUTPUT/ 2>/dev/null || true
```

#### Method 2: Using latexmk (Recommended)
```bash
# Navigate to project directory
cd /path/to/ug-thesis-template/

# Create output directory
mkdir -p OUTPUT

# Automated compilation with latexmk
latexmk -pdf -pdflatex="pdflatex -interaction=nonstopmode" main.tex

# Continuous preview mode (auto-recompile on changes)
latexmk -pdf -pvc -pdflatex="pdflatex -interaction=nonstopmode" main.tex

# Clean auxiliary files
latexmk -c

# Clean all generated files including PDF
latexmk -C

# Move files to OUTPUT directory
mv main.pdf OUTPUT/
mv *.aux *.bbl *.blg *.log *.toc *.lof *.lot *.fls *.fdb_latexmk \
   OUTPUT/ 2>/dev/null || true
```

#### Optional: Create .latexmkrc Configuration
Create a `.latexmkrc` file in the project root:

```perl
# .latexmkrc configuration file
$pdf_mode = 1;                    # Generate PDF using pdflatex
$bibtex_use = 2;                  # Run bibtex when needed
$pdflatex = 'pdflatex -interaction=nonstopmode -synctex=1 %O %S';
$out_dir = 'OUTPUT';              # Output directory
$aux_dir = 'OUTPUT';              # Auxiliary files directory
$clean_ext = 'bbl aux blg idx ilg ind lof lot out toc synctex.gz 
              fdb_latexmk fls log';
@default_files = ('main.tex');   # Default main file
```

Then simply run:
```bash
latexmk
```

### 🌐 Online Compilation (Overleaf)

1. **Import Template**: Use the Overleaf template link: [Overleaf template link will be added here]
2. **Set Compiler**: Configure to use `pdfLaTeX` (2023/24 or above Dont use 2025 before its stable next update) or `latexmk`
3. **Bibliography Engine**: Set to `bibtex`
4. **Collaborate**: Share with team members for multi-student projects

---

## 🎯 Degree-Specific Configurations

### 🎓 Undergraduate (UG) Requirements

- **Maximum Students**: 3 students per group
- **Author Biography**: Not included
- **Degree Type**: Bachelor of Technology (B. Tech.)
- **Paper Code**: As per department guidelines

```latex
% Configuration for UG
\NumberOfStudents{3}
\DegreeType{Bachelor of Technology (B. Tech.)}

% Exclude author biography
%\include{Backmatter/AuthorBio} % Commented out for UG
```

### 🎓 Postgraduate (PG) Requirements

- **Number of Students**: 1 student only
- **Author Biography**: Mandatory
- **Degree Type**: Master of Technology (M. Tech.)

```latex
% Configuration for PG
\NumberOfStudents{1}
\DegreeType{Master of Technology (M. Tech.)}

% Include author biography
\include{Backmatter/AuthorBio} % Required for PG
```

### 🎓 Doctoral (PhD) Requirements

- **Number of Students**: 1 student only
- **Author Biography**: Mandatory with detailed research profile
- **Degree Type**: Doctor of Philosophy (Ph.D.)
- **Publications List**: Comprehensive list of published research papers

```latex
% Configuration for PhD
\NumberOfStudents{1}
\DegreeType{Doctor of Philosophy (Ph.D.)}

% Include author biography and publications
\include{Backmatter/PublicationsList}
\include{Backmatter/AuthorBio} % Required for PhD
```

---

## 💡 Advanced Features

### 🖥️ MATLAB Code Highlighting

```latex
\begin{lstlisting}[style=Matlab-editor]
function result = myFunction(input)
    % Your MATLAB code here
    result = input * 2;
    fprintf('Result: %f\n', result);
end
\end{lstlisting}
```

### 📊 Figure and Table Management

```latex
\begin{figure}[H]
    \centering
    \includegraphics[width=0.8\textwidth]{Chapter01/figure_name.png}
    \caption{Descriptive caption for the figure}
    \label{fig:figurelabel}
\end{figure}
```

### 🧮 Mathematical Expressions

```latex
\begin{equation}
    P = V \cdot I \cdot \cos(\phi)
    \label{eq:power}
\end{equation}
```

### 🔄 Supervisor College Flexibility

The template now supports specifying different colleges for supervisors and co-supervisors:

```latex
\Supervisor{Dr. External Supervisor}
\SupervisorCollege{Indian Institute of Technology Kharagpur}

\CoSupervisor{Dr. Internal Guide}
\CoSupervisorCollege{National Institute Of Technology Durgapur}
```

---

## 🛠️ Customization

### 🎨 Colors and Styling
Modify colors in `thesis.cls`:
```latex
\definecolor{darkblue}{rgb}{0.0, 0.0, 0.5}  % Custom colors
```

### 📐 Page Layout
Adjust geometry in `thesis.cls`:
```latex
\RequirePackage[
    a4paper,
    textwidth=15.5cm,
    textheight=23cm,
    left=3cm,
    right=2.5cm,
    % ... other settings
]{geometry}
```

---

## 🏆 Best Practices

### ✅ Recommended Practices

1. **Consistent Naming**: Use descriptive file names with chapter prefixes
2. **Image Resolution**: Maintain high-resolution images (300 DPI minimum)
3. **Backup Strategy**: Regular backup using version control systems (Git)
4. **Validation Testing**: Periodic compilation testing to identify issues early
5. **Use latexmk**: Automated compilation saves time and reduces errors

### ❌ Common Issues and Solutions

| Issue | Solution |
|-------|----------|
| Missing Packages | `sudo pacman -S texlive-most texlive-bibtexextra` |
| File Path Issues | Verify relative paths for figures and includes |
| Encoding Problems | Ensure UTF-8 encoding for all text files |
| Bibliography Errors | Check reference format and .bib file syntax |
| latexmk Issues | Clear auxiliary files using `latexmk -C` |
| Compilation Hangs | Use `-interaction=nonstopmode` flag |

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](https://github.com/KingsukMajumdar/NITDGP-Thesis-Template-Unofficial/blob/main/LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Kingsuk Majumdar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

### 🔖 Third-Party Components

- **mcode.sty**: BSD License (Florian Knorn)
- **Standard LaTeX Packages**: Various open-source licenses
- **TeX Live Distribution**: TeX Users Group License
- **latexmk**: GNU General Public License

---

## 🤝 Contributing

We welcome contributions! Please see our contributing guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### 🐛 Reporting Issues

When reporting issues, please include:
- LaTeX distribution and version
- Operating system
- Complete error messages
- Minimal example that reproduces the issue

---

## 📞 Support & Contact

- **GitHub Issues**: [Create an issue](https://github.com/) for bug reports and feature requests
- **YouTube Channel**: [Learn With Kingsuk](https://www.youtube.com/@LearnWithKingsuk)
- **Institution**: National Institute Of Technology Durgapur
- **Department**: Electrical Engineering

**Hashtags:** #LearnWithKingsuk #134rnW17hK1N65uk #ElectricalEngineering #Python #Engineering #NITDGP #TechnicalEducation #EngineeringStudent #PowerSystems #Tutorial

---

## 🔗 Quick Links

| Platform             | Link                                                                                                  | Description            |
| -------------------- | ----------------------------------------------------------------------------------------------------- | ---------------------- |
| 🐙 **GitHub**        | [GitHub repo](https://github.com/KingsukMajumdar/NITDGP-Thesis-Template-Unofficial.git)               | Source code and issues |
| 📝 **Overleaf**      | Manually upload (for free account)                                                                    | Online template        |
| 📚 **Documentation** | [README.md](https://github.com/KingsukMajumdar/NITDGP-Thesis-Template-Unofficial/blob/main/README.md) | Detailed documentation |
| 🏫 **Institution**   | [NIT Durgapur Website](https://nitdgp.ac.in/)                                                         | Institute website      |
| 📺 **YouTube**       | [Learn With Kingsuk](https://www.youtube.com/@LearnWithKingsuk)                                       | Video tutorials        |

---

## 🙏 Acknowledgments

- **National Institute Of Technology Durgapur** for institutional support and academic excellence
- **Prof. Subrata Banerjee, Professor, EE, NIT Durgapur** (my supervisor) for giving permission to write thesis in LaTeX during my M. Tech. and Ph.D.
- **Florian Knorn** for the excellent mcode.sty package
- **LaTeX Community** for comprehensive packages and documentation
- **Contributors** who helped improve this template
---

## 📈 Version History

- **V1.0** (2025-10-18): Initial release for NIT Durgapur
  - Added latexmk support
  - Added flexible supervisor college configuration
  - Enhanced for UG/PG/PhD requirements
  - Updated institutional branding and information

---

## 🎯 Future Enhancements

- [ ] Add support for multiple co-supervisors
- [ ] Include templates for thesis proposal
- [ ] Add dark mode theme option
- [ ] Create video tutorials for common tasks
- [ ] Develop GUI-based configuration tool
- [ ] Add support for additional programming languages
- [ ] Include thesis checklist and submission guidelines

---

<div align="center">

**⭐ Star this repository if it helped you! ⭐**

*Made with ❤️ for students and researchers of National Institute of Technology Durgapur*

**An Initiative by an Alumnus**

With Regards
Kingsuk Majumdar



[![GitHub followers](https://img.shields.io/github/followers/KingsukMajumdar?style=social)](https://github.com/KingsukMajumdar)
[![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCo2Rho6ypq7IkxaKwByWQRA?style=social)](https://youtube.com/@LearnWithKingsuk)
</div>
