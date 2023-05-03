# Gitignore Cheet Sheet

## Gitignore

### What is gitignore?

Gitignore is a file that tells git which files to ignore. It is useful when you have files that you don't want to push to your repository.

### How to use gitignore?

1. Create a file called `.gitignore` in the root directory of your repository.

2. Add the files you want to ignore to the file.

3. Commit and push the file to your repository.

### Example

```
# Ignore all .a files
*.a

# But do track lib.a, even though you're ignoring .a files above

patterns in .gitignore files are relative to the location of the .gitignore file. 
```

# Patterns

        Patterns | Explanation/matches | Example
        ------------ | ------------- | -------------
        name.file | Matches a file called name.file | /name.file 
        **/logs | Matches any file or directory called logs | /logs, /a/logs, /a/b/logs
        foo/ | Matches directories called foo | /foo, /a/foo, /a/b/foo
        name/ | Matches directories called name and all files in them | /name, /name/file.txt,      
         /name/a/b/c/file.txt
        **/name | Matches any file or directory called name | /name, /a/name, /a/b/name, /a/b/c/name
        *.file | Matches any file ending in .file | /a.file, /b.file, /a/b.file
        temp.* | Matches any file beginning with temp. | /temp.a, /temp.b, /a/temp.c