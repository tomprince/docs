## stop

    Usage: hyper stop [OPTIONS] CONTAINER

    Stop a container

      --help=false       Print usage
      -t, --time=10      Seconds to wait for stop before killing it

The main process inside the container will receive `SIGTERM`, and after a grace
period, `SIGKILL`.
