---
layout: post
title: "Research"
author: "Vinnie"
permalink: /research/
---

User and device behavior

Modern computing devices are equipped with an unprecedented range of sensing capabilities, enabling novel insights to be gained about the user, the device, and the environment. While these insights enable applications to be more responsive to user actions, operate with greater efficiency, and react to complex stimuli, heterogeneous sensing capabilities have also led to a new class of side channel attacks aimed to undermine user privacy and compartmentalized security. Interestingly, the patterns that emerge from sensed input, such as through keyboard, microphone, and numerous other modalities, can be used to both increase security, such as by continuously verifying the user's identity, and decrease security, with cross-sensor eavesdropping being a prime example. These types of applications are largely enabled by two related phenomena in human-computer interaction (HCI):

Between-user variability: Individual users exhibit unique and identifiable behavior interacting with a computer interface, resulting from idiosyncratic factors such as motor skill and physiology. These differences can be observed during interaction with keyboard, touchscreen, and other HCI modalities, and as the events propagate to the network level, user identification can be performed passively and remotely.

Between-user consistency: An entire population may operate a computer interface within certain constraints, enabling an adversary to make general inferences about a particular user's actions. HCI largely follows general rules, such as Fitts’ Law in navigating the mouse pointer on a computer screen and the inverse scaling of keystroke latencies with key distance: shorter time intervals usually correspond to keys that are far apart compared to longer time intervals between neighboring keys.

These two phenomena are generally seen as opposing one another, and quantifying their tradeoff remains an active area of my current research. I am especially interested in human-based timing side channels, such as the ability to discern keyboard keys based on time intervals. This is analogous to the way a timing side channel enables encryption keys to be efficiently recovered, relying on the notion that certain math operations take shorter or longer to complete based on the encryption key bit pattern.

Privacy-enabling technologies

The interactive real-time client/server model, where the role of the client is to transmit the user's actions to the server in an event-driven fashion, represents a rather broad class of web-based applications. Such applications, including ssh in interactive mode and Google search, capture and transmit user input events, such as keystrokes and touchscreen events, in real time. As these events propagate to the network level, an adversary can remotely observe user and device behavior without the victim's cooperation or knowledge. This can lead to keystroke dynamics-based remote user identification, a well-established threat to anonymizing technologies, and temporal keylogging, a threat which potentially remains underdeveloped at this point. In order to mitigate these threats, my work aims to develop methods of behavior obfuscation that conceal user identity and application content. This must be performed online and without excessively degrading the responsiveness of the application, otherwise this method of defense becomes unusable. Closely related is the problem of behavior spoofing, in which an adversary modifies their behavior in order to mimic a particular user or device.

Emerging computer architectures

Computing architectures are on the cusp of a fundamental shift towards concurrency as sequential models struggle to process large amounts of data in real time. Alongside this shift, a range of non-von Neumann architectures, some designed to operate within size, weight, and power constrained environments, have begun to emerge. Many of these architectures are inspired by the mammalian brain, built on principles such as massive parallelism and event-driven computation. However, programming such architectures remains a challenge and their impact to security and privacy is currently unclear. My research in emerging computer architectures addresses two different areas aimed to increase the programmability and application space of neuromorphic architectures.

Leverage emerging non-von Neumann architectures to solve computationally-hard optimization and security problems, especially those which are unattainable or inefficient on a von Neumann architecture. This path is enabled by the unique characteristics of emerging architectures, such as the massive parallelism and inherent stochasticity of some neuromorphic processors, upon which new classes of algorithms designed to solve computationally-hard problems are built. I am especially interested in how neuromorphic architectures can be used to efficiently factor integers.

The integration of symbolic and subsymbolic processing on a unified neuromorphic architecture. Spiking neural networks (SNN) traditionally operate on numerical data (subsymbolic), but can we configure an SNN to operate on or with structured data (symbolic)? The work in this area aims to develop addressable and structured memory in SNNs which can be integrated with both symbolic processing and learning-based systems on current and near-future neuromorphic architectures.
