# teaching-js
A repository for teaching javascript from the textbook Javascript The Definitive Guide 7th Edition.

## Structure
Each chapter directory will contain an exercises.txt file with a group of numbered exercises. 

Students should clone this repo (see Using Git section below) and put their solutions to each exercise either as a single named file (ex: 3-5.js for chapter 3 exercise 5), or if a solution is split into multiple files create a directory (ex: 3-5) with your code in it. You should also add questions you have to the questions.txt document in each chapter directory as you read. I will go through and answer them when I see them in the repo or when you notify me in person. This book does assume some knowledge so you should add questions for anything you don't understand or previously have experience with that the book assumes you know.

It is highly recommended to have a computer nearby when reading the book so you can try out what you're reading and keep a document with questions you think of so you don't forget what they were when we meet in person and I can answer them ahead of time.

Make sure to push your changes if you work on any exercises or add any questions.

Unless explicitly stated, you can choose to implement your code using a web browser or node. I recommend using node for most optional problems.

## Using the Terminal
To change directories
```bash
    cd [path] # Changes directory to specified path
```

To list directory contents
```bash
    ls # lists current dir contents
    ls [path]
```

To run node on a javascript file
```bash
    node program.js
```

### Redirection and Piping
This isn't super important to know but I personally find it very useful. It's also used occassionally by the author of the book.

You can take the contents of a file and use them as input to a program instead of having the user type in the input themselves. This is done using a redirection operator ```<```.
```bash
    node program.js < my-input.txt
```

Similarly you can change the output of your program to redirect into a file instead of to the console using the ```>``` operator.
```bash
    node program.js > my-output.txt
```

If you want to take the output of one program and use it as the input of another program you can use the pipe operator ```|```. In this example I'm piping the output of program1.js into program2.js and redirecting all the output of program2.js into my_output.txt.
```bash
    node program1.js | node program2.js > my_output.txt
```

## Using Git
To clone the repo to your local machine run the command:
```bash
    git clone https://github.com/CarlSchader/teaching.js.git
```

To commit and push your changes run:
```bash
    git add .
    git commit -m "Some commit message such as: finished 3-5.js"
    git push origin main
```