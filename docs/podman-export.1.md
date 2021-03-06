% podman(1) podman-export - Simple tool to export a container's filesystem as a tarball
% Urvashi Mohnani
# podman-export "1" "July 2017" "podman"

## NAME
podman export - Export container's filesystem contents as a tar archive

## SYNOPSIS
**podman export**
**CONTAINER**
[**--output**|**-o**]
[**--help**|**-h**]

## DESCRIPTION
**podman export** exports the filesystem of a container and saves it as a tarball
on the local machine. **podman export** writes to STDOUT by default and can be
redirected to a file using the **output flag**.

**podman [GLOBAL OPTIONS]**

**podman export [GLOBAL OPTIONS]**

**podman export [OPTIONS] CONTAINER**

## OPTIONS

**--output, -o**
Write to a file, default is STDOUT

## EXAMPLES

```
# podman export -o redis-container.tar 883504668ec465463bc0fe7e63d53154ac3b696ea8d7b233748918664ea90e57
```

```
# podman export > redis-container.tar 883504668ec465463bc0fe7e63d53154ac3b696ea8d7b233748918664ea90e57
```

## SEE ALSO
podman(1), podman-import(1), crio(8), crio.conf(5)

## HISTORY
August 2017, Originally compiled by Urvashi Mohnani <umohnani@redhat.com>
