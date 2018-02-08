# Taskserver Setup

This guide leads you through all the necessary steps to setup your own Taskserver to sync your Taskwarrior-tasks.

Please follow the steps **carefully** and **note** all things you do differently.

---

## Preparation - Backup Your Data

Let's reinforce a good habit and make a backup copy of your data first. Here is a very easy way to backup your data:

```bash
$ cd ~/.task
$ tar czf task-backup-$(date +'%Y%m%d').tar.gz *
```

Now move that file to somewhere safe. All software contains bugs, so make regular backups.

---

## Attention

This is not only due to a good habit, we will modify your data, so a backup is highly recommended.
