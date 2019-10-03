---
title: 'Chapter Title Here'
description: 'Chapter description goes here.'
---

## Example coding exercise

```yaml
type: NormalExercise
key: e8c1edbe67
lang: python
xp: 100
skills: 2
```

This is an example exercise.

`@instructions`


`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```

---

## Insert exercise title here

```yaml
type: IDEExercise
key: c38a470a06
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
- permission: 755
  open: false
  path: foo.py
  content: |+
    from project.hello_world import greet
    greet()

    print("Hello World!")


```

`@solution`
```{python}
- path: foo.py
  open: true
  content: |
    def greet():
        print("Hello World!")
- path: bar.py
  content: |
    from project.hello_world import greet
    greet()

    print("Hello World!")

```

`@sct`
```{python}
# Documentation for reference: https://pythonwhat.readthedocs.io/en/latest/reference.html#checking-files.

# Relevant methods:
# - check_file: Checks if a file exists.
# - has_dir: Check if a directory exists.
# - has_commands: Check if bash history has a matching command.

# Example SCT using check_file() and run()
# add SCT parts after run() as you normally do.
Ex().check_file("path_to_file", solution_code="a=1").run()
```
