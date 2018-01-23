# Debugging

## ASAN

There are several ways to use RetroArch in conjunction with ASAN.

**For detecting memory leaks**
> make DEBUG=1 SANITIZER=address,undefined

**For detecting thread errors**
> make DEBUG=1 SANITIZER=thread,undefined
