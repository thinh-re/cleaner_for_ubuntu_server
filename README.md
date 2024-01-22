# Best practices to free up disk memory

You are using an Ubuntu Server, someday you notice that the server is running out of space. To help keep your space under control. Here are several ways you might need to do this every month.

## Clean up pip's cache

```Shell
pip cache purge
```

## Clean up Anaconda's cache

```Shell
conda clean -a
```

## Clean up Docker usage

This will remove:

- all stopped containers
- all networks not used by at least one container
- all images without at least one container associated with them
- all build cache

```Shell
sudo docker system prune -a
```

You can remove build cache only.
```Shell
// Check disk usage first
sudo docker system df 

// Remove build cache
sudo docker builder prune -a
```

## Clean NPM's cache

```Shell
npm cache clean --force 
```
