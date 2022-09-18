- [X] List all HDFS Commands

```bash
hadoop fs
hdfs dfs
```

- [X] Basic usage for any command

```bash
hadoop fs -usage ls
```

```
hadoop fs -put dataFiles/* practice/retail_db/
hadoop fs -ls -R practice/retail_db
```

- [X] List/Sort files in HDFS
- Command - ls
  - Use a pattern to select
  - -R recursively list the contents of directories
  - -C Display the paths of files and directories only
- By default it sorts in ascending order by name
  - ls -r Reverse the order of the sorte
  - ls -S Sort files by size
  - ls -t Sort files by modification time (most recent first)

- [X] Creating/Deleting Directories in HDFS
- Command: rmdir
  - Remove Directory if it is empty
- Command: rm
  - rm remove files
  - -r recursively deletes directories
  - -skipTrash bypasses trash, if enabled
  - -f, no error message even if file does not exist. Check with Unix command $?.
- command: mkdir
  - Create directory
  - -p do not fail if the directory already exists