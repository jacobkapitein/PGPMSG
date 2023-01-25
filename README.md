# 🔐 PGPMSG (Work In Progress)

> PGPMSG is a messaging service for Android for sending secure End-to-end encrypted messages using PGP.

# Personal Goals

- Get more knowledge in secure communication and e2e encryption
- Get more knowledge in OpenPGP
- Maintain & update skills in React (Native)
- Update my skills in git and deployments

# Project Goals

**Must haves**
- Realtime Secure messaging between 2 persons (encryption and signing)
- Realtime push notifications like Signal, Telegram or WhatsApp
- No registration
- No saving of **any** user data
- Self-hostable for anyone, while maintaining a single app

I want to build an app which makes it possible for 2 persons to securely communicate without relying on any services not in your control. This must mean that any required service is self-hostable. It must also no use any services which might compromise user data. This means any user data will not be stored in any database at all.

I also don't want to use any services like Google Cloud, Azure or other services which might be in control of your data. Everything server-side will be able to run in Docker and will be easy to set up for anyone. I will also not use any service like Firebase for push notifications. This will be a challenge, because it's hard to manage an app in the background on Android due to limitations with power management put on by the OS.

Lastly, I don't want any complicated registration for a user. You don't have to fill in your name or email address anywhere.

**Could haves**
- Sending images, videos and files
- Secure group chats

This is just extra. It is possible, but my main focus are the personal goals and I think those can be accomplished with only the must haves.

**Won't haves**
- Backups of chats

# Project Management

I won't manage this project in any way. I have a board for myself on which I manage my tasks, but I will do whatever I feel like doing.

Any commit will be signed with my PGP key, so each commit should have a "verified" badge next to it. I will use conventional commits to learn to integrate it with semver. Version 1.0.0 is a long way to go tho as the project is still empty as I'm writing this.

# Possible Challenges

## Storage of chats
Storage of chats must also be done securely and locally on a device. I think this will be a challenge as it must be encrypted in some way. I will probably do this with a user provided password, so I don't have to save some key on the device in the secured storage.

## Push notifications

I expect this to be a challenge as I have no idea how to do this yet. I know both Android and iOS *really* restrict background apps with the network, so I probably won't be able to keep a WebSocket open.
