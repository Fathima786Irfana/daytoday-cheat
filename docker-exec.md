## 1. **Docker : Open a shell inside a running container**

* The command `docker exec -it` is used to access a running Docker container's shell in interactive mode. It will open a Pseudo terminal so you can execute commands inside the container as if you were logged into a separate terminal session.

---

**Basic Syntax**

```
docker exec -it <container_name_or_id> <shell>
```
Example shells: `sh`, `bash` (depending on the container)

---

**Options**

| Options    | Description|
| --------- |------------------- |
| `-d, --detach`  | Detached mode: run command in the background |
| `-i, --interactive`  | Keep STDIN open even if not attached |
| `-t, --tty`  |   Allocate a pseudo-TTY|
| `-w, --workdir`  | Working directory inside the container |

---

**Common Patterns or Use Cases**

```
# With Bash Shell and container name
docker exec -it mycontainer bash

# With sh Shell and container id
docker exec -it cbc1edd86331 sh
```