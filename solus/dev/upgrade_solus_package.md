# Upgrade Solus Package

1. Update package.yml

```bash
yupdate $VERSION $URL_TO_TARBALL
```

2. Build the binary

```bash
make
```

3. Install the binary

```bash
sudo eopkg -it $BINARY
```

4. Run tests

5. Commit changes

```
git commit -p
```

6. Submit patch

```
arc diff
```
