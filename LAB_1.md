### AI Laboratory work 1: Machine Reasoning.

# The task description.

In this task you are going to create a 2d cube world with a grabing hook that will have to place one cube on another, and then answer reasoning questions being able to explain it's action.

# The requirements of the project.
1. At the beginning provide the length and width of the world matrix.
2. Create the empty matrix using the provided values.
3. Ask the use to introduce several blocks coordinates and place them in the matrix, take it into account that the block shouldn't stay in the air.
4. Create the Logging list where all the actions will be added during the execution of the algorithm.
5. Write three functions that will implement the following actions:
   * grasp - will make the grabbing hook to grasp the provided block
     grasp(block):
   * move - will place block_1 onto block_2 and will get rid of additional block depending on the case.
     move(block_1, block_2, get_rid_of=False) - the get_rid_of parameter will control if the block need their tops removed.
   * put_on - the main function that will put block_1 on block_2 using the grasp and move functions
     put_on(block_1, block_2)
6. Write a cmd_handler function that will take in and infinite look questions and will answer them based on the logging list.
   The cmd_handler should be able to answer the following questions:
   * Why did you clear top of x
   * Why did you grasp X
   * Why did you get rid of X
   * Why did you put X on Y
   * How did you cleared the top of X
   * How did you grasp X
   * How did you get rid of X
   * How did yoy put X on Y
   * kill or quit - will quit the whole program.
7. Call the put_on algorithm.
8. Call the cmd_handler to ask questions about how the algorithm works.
9. Additionally if you want during the running of the put_on algorithm at every step you can show/print out the cude world.