# SMAT 4 — MATLAB-compatible scientific web workspace

SMAT uses GNU Octave as its scientific execution engine.

Includes:
- MATLAB/Octave `.m` scripts
- matrices, vectors and numerical calculations
- functions and local functions
- ODE solvers such as `ode45`
- 2-D and 3-D plotting
- PNG figure export
- Command Window output
- New / Save / Save As
- mobile responsive UI
- Docker deployment

Important: GNU Octave is broadly MATLAB-compatible but is not proprietary MATLAB. Some MATLAB-only APIs, proprietary toolboxes, Simulink and App Designer are not included.

## Docker

docker build -t smat .
docker run --rm -p 3000:3000 smat

Open http://localhost:3000

## Security

The example blocks several obvious OS commands and has an execution timeout. This is not a complete security sandbox for arbitrary public users. A production public service should isolate executions in separate containers/VMs with CPU, memory, filesystem and process limits.
