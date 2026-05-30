# Linux I/O and Pipes

## stdin

Standard Input.

Receives data from the user.

Example:

read name

---

## stdout

Standard Output.

Displays normal output.

Example:

echo "Hello"

---

## stderr

Standard Error.

Displays error messages.

Example:

ls file_that_does_not_exist

---

## Redirection

Redirect output to a file.

Example:

echo "Hello" > file.txt

---

## Pipe

Symbol:

|

Used to send output from one command to another.

Example:

ls | wc -l

---

## Practical Example

ps aux | grep firefox

Displays only processes containing the word firefox.