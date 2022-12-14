# Installation

## Python server and example agent

Create a virtual environment to house dependencies for this project. This makes
it easy to remove all the dependencies later as the virtual environment can
just be deleted.

### Venv
If you want to use venv to make a virtual environment:

```
python3 -m venv /path/to/env
```

Activate the environment. You'll need to do this every time you open your terminal back up.

```
source /path/to/env/bin/activate
```

### Conda
If you want to use conda to make a virtual environment:

```
conda create -n env_name
```

To activate:

```
conda activate env_name
```

Install the python dependencies.
```
pip install -r requirements.txt
```

# Running

You will need to start the server and a single agent in two separate terminals
so they are both running at the same time. Also, if one dies you will have to
close and restart the other one as well or it won't reconnect.

## Inverted pendulum server

To run the server with animation of the pendulum enabled

```
python inverted_pendulum_server.py --animate
```

To run as fast as possible, omit the animate argument

## Python example agent

```
python example_agent.py
```

To run from a save file, use the following command

./polarAgent.py Outfiles/FileName.json 0

