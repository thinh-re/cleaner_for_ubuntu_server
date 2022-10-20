# Cleaner for Ubuntu Server

You are using Ubuntu Server, someday you notice that the server is running out of space. To help keep your space under control. Here are some steps you might need to do every month.

## Clean pip's cache

```Shell
pip cache purge
```

## Clean Anaconda's cache

```Shell
conda clean -a
```

## Clean Docker

```Shell
sudo docker system prune -a
```