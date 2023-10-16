This is is a simple program that parses the requirements for the Phoenix CubeSat and outputs a graph in DOT format.

# Background

The University of Arizon in Phoenix has developed a CubeSat satellite and documented the requirements and design:

https://phxcubesat.asu.edu

The requirements spreadsheet is included with this project but can also be found here:

https://phxcubesat.asu.edu/sites/default/files/general/phoenix_requirements.xlsx


# Setup

Similar to previous project, the setup includes creating a virtual environment and then installing the project dependencies:

```bash
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

Note, that this project only uses the `openpyxl` library to parse the spreadsheet.


# Run

The parser can be executed via the command line by running>

```bash
python app/requirements_parser.py
```

or by running `Run Parser` from within VSCode.

The program will parse the requirements spreadsheet in the `static` folder and output the graph in DOT notation. Copy the graph into a visual editor, such as:

https://dreampuf.github.io/GraphvizOnline

Now inspect the graph for requirements traceability issues.