

# How to Capture Network Traffic: SPAN vs TAP

## 1. What are the differences between SPAN and TAP?

   According to Accedian's blog, SPAN, or port mirroring, is a method where traffic from one or more ports of a switch is copied to another port. A network TAP (Terminal Access Point) is a device that passively captures traffic between two network points. SPAN is software-based and can be managed remotely, while TAP is hardware-based and provides a dedicated monitoring port.

## 2. What types of network devices can support network traffic mirroring?

   Most network switches support port mirroring or SPAN as it is a feature embedded in these devices. TAPs, on the other hand, are separate hardware devices placed between network points to capture traffic passively.

## 3. How can network traffic mirroring be used for network security?
 Network traffic mirroring can be used for security applications as it allows for the monitoring of traffic for anomalies or malicious activity. TAPs are especially useful as they are non-obtrusive, undetectable on the network, and can handle full-duplex networks, maintaining traffic even if power is lost.

## 4. Are there any legal or ethical considerations when using network traffic mirroring?

   While the article from Accedian does not specifically address legal or ethical considerations, it is generally understood that network traffic mirroring should be conducted in compliance with laws and regulations regarding privacy and data protection. Unauthorized interception or monitoring of network traffic can lead to legal penalties and ethical breaches.