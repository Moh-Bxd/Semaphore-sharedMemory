# Semaphore and Shared Memory Project <Syc 2023 second lab>

This project demonstrates inter-process communication (IPC) using semaphores and shared memory in C. The application simulates a swimming pool scenario with swimmers managing shared resources (changing cabins and baskets) using synchronization mechanisms.

## Features

- **Semaphores**: Used to synchronize access to shared resources (changing cabins and baskets).
- **Shared Memory**: Used to store the state of resources (number of available baskets and cabins).
- **Process Management**: Forks child processes to simulate swimmers.
- **Resource Allocation**: Ensures that swimmers request, use, and release resources in a controlled manner.

## Code Structure

### Files

1. **main.c**: 
   - Initializes semaphores and shared memory.
   - Spawns child processes to simulate swimmers.
   - Manages cleanup of semaphores and shared memory.

2. **nag.c**: 
   - Represents the logic for each swimmer process.
   - Simulates the swimmer's behavior, including requesting and releasing resources, changing clothes, and swimming.


## Usage

### Compilation

Use the following command to compile the project:

```bash
gcc main.c -o main
gcc nag.c -o nag
