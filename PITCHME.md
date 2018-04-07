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

---

## Preparation - Choose A  Machine

A suitable machine to run your Taskserver is one that is always available. If you have such a machine, or have access to a hosted machine, that is ideal.

If your machine is not continuously available, it can still be a suitable Taskserver because the sync mechanism doesn't require continuous access. When a client cannot sync, it simply accumulates local, unpropagated changes until it can sync.

A laptop is a poor choice for a Taskserver host.
