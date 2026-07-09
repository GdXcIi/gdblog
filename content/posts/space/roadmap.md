+++
date = '2026-07-08T12:51:27+02:00'
draft = true
title = 'Roadmap of Space'
+++

## Roadmap to 1.0 version

Hello everyone!

Today I'm presenting you my roadmap to Space 1.0 stable release, which should release on April 12, 2029.

### v0.1 - A minimalistic (but functional!) microkernel

0.1 version won't be very very impressive. It will just be a microkernel that works but which is very minimalistic.

This version will include:
- a minimalistic memory manager
- a minimalistic logging system (but kernel panic will be working!)
- a few syscalls for only necessary things:
 - `send_ipc` = asks the microkernel to send an IPC
 - `wait_ipc` = says the microkernel that we wait for an IPC (practical for the scheduler)
 - `alloc` = asks the microkernel to allocate memory
 - `free` = asks the microkernel to free memory
 - `get_hardware_perms` = asks the microkernel to get a hardware permission (just a placeholder because 0.1 won't include security and permissions logic)
 - `get_ipc_perms` = asks the microkernel to get an ipc permission (idem)
- no security and permissions logic (this is not critical for the functionment of the microkernel)
- a minimalistic ipc-centric scheduler

### v0.2 - Stabilization of the 0.1

This version won't bring a lot, just stabilizations of the v0.1.

### v0.3 - Improvement of the IPC logics

This version will just improve IPC logics and add some features for IPC logics.

### v0.4 - Stabilization of the 0.3

Just stabilizations and bug fixes.

### v0.5 - A better memory manager!

Improvements of the memory manager, optimizations, new and better abstractions to alloc and free...

### v0.6 - Stabilization of the 0.5

No more to say.

### v0.7 - A complete log manager

Improvements of the log manager with better abstractions, optimizations...

### v0.8 - Stabilizations of the 0.7

I think I don't need to say more.

### v0.9 - Improvement of the scheduler with a much better algorithm!

Improvements of the algorithm of the scheduler, with optimizations and more solidity, etc...

### v0.10 - Stabilization of the 0.9

Just stabilizations of the 0.9: optimizations, bug fixes...

### v0.11 - Introducing security and capabilities!

This will be a big step in the history of the micokernel: introducing all the main logic of security and hardware and ipc capabilities!

### v0.12 - Stabilzations of the 0.11

Ok just stabilzations: bug fixes, optimizations, correcting some security fails...

### v0.13 - Stabilizations of all the microkernel

Ok just global stabilizations...

### v1.0 - Space 1.0 stable release!

Introducing Space 1.0 stable release! Space will finally be out!

---

You may have noticed that every version is followed by a stabilization version. That is because the 0.x versions are the bases of all the next of the microkernel, so we need stability for each new feature. 
