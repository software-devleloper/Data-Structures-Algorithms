How does Backtracking work ?
When you need to check all the solutions or iterate thorough each possible solution, we use backtracking. 

When do you use Backtracking ? 
Common problems where we use this - Solving puzzles like Sudoku, Maze, Combinatorial problems - permutations, combinations, Job Scheduling.

Basic Code structure : 
Choose a step, explore further steps, backtrack on this step. 

function backtrack(candidate_solution):
    if candidate_solution is a complete solution:
        output candidate_solution
        return
    
    for each option in choices from current state:
        if option is valid:
            add option to candidate_solution
            backtrack(candidate_solution)
            remove option from candidate_solution  // undo choice (backtrack)


