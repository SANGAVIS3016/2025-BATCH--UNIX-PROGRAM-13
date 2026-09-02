# Linux Assignment: Add a User and Display User Details

## Aim

Create a Linux user named `jeevitha` and display the details of the user using the `id` command.

## Learning Objectives

By completing this assignment, you will learn how to:

* Create a Linux user using `useradd`.
* Verify whether a user exists.
* Display user and group information using the `id` command.
* Execute Linux commands from a terminal.
* Work with shell scripts and GitHub Actions.

## Algorithm

1. Open the Terminal on a Linux machine.
2. Create a user named `jeevitha` using the `useradd` command.
3. Display the details of `jeevitha` using the `id` command.
4. Verify that the user was created successfully.
5. Save your solution and push it to GitHub.
6. GitHub Actions will automatically run the tests.

## Expected Commands

The basic Linux commands required for this assignment are:

```bash
sudo useradd jeevitha
id jeevitha
```

> Note: The automated environment runs with sufficient privileges, so your script should not depend on interactively entering a sudo password.

## Student Task

Open:

```text
starter/solution.sh
```

Complete the script so that it:

1. Creates the user `jeevitha`.
2. Does not fail if the user already exists.
3. Displays the details of `jeevitha` using the `id` command.
4. Returns a successful exit status when the task is completed correctly.

## Example Output

A successful execution may produce output similar to:

```text
uid=1001(jeevitha) gid=1001(jeevitha) groups=1001(jeevitha)
```

The UID, GID, and group numbers may be different on different Linux systems.

## Submission Instructions

1. Clone or accept the assignment repository.
2. Open `starter/solution.sh`.
3. Complete the script.
4. Test it locally on a Linux system.
5. Commit your changes.

Example:

```bash
git add starter/solution.sh
git commit -m "Complete useradd assignment"
git push
```

6. Check the **Actions** tab on GitHub.
7. Your submission is automatically tested.

## Grading

| Test                                       |   Marks |
| ------------------------------------------ | ------: |
| Correctly creates `jeevitha`               |      40 |
| User exists after execution                |      20 |
| Correctly displays user details using `id` |      20 |
| Script executes successfully               |      10 |
| Code quality/basic shell scripting         |      10 |
| **Total**                                  | **100** |

## Important Requirements

* The username must be exactly `jeevitha`.
* The solution must use the Linux `useradd` command.
* The solution must use the Linux `id` command to display the user's details.
* Do not hard-code fake `id` output.
* Do not modify the test files.
* Do not modify the GitHub Actions workflow to bypass the tests.

## Academic Integrity

Write and test your own solution. You may refer to Linux documentation and course materials to understand the commands.

## Local Testing

You can execute the solution with:

```bash
bash starter/solution.sh
```

Then verify the user manually:

```bash
id jeevitha
```

## Result

After successful completion, the system should contain a user named `jeevitha`, and the `id` command should display information about that user.
