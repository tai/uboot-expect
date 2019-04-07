# uboot-expect
Control U-Boot console with Expect (Python pexpect)

## Usage

Usage: uboot-expect [option] <input-files...>
Options:
  -D|--debug <level>  : Debug level ('INFO', 'DEBUG', ...)
  -p|--prompt <prompt>: Prompt to wait for (ex: "U-Boot>")
  -s|--shell <command>: Command to interact (ex: "cu -s 9600 -l /dev/ttyS1")
  -t|--timeout <secs> : Timeout in seconds
Example:
  $ uboot-expect -p 'CNCl800L>' -s 'cu -s 115200 -l /dev/ttyUSB6' input.cmd
