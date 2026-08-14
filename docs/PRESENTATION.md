### VIAVI SecurePNT EdgeGM 7000

This is a master clock designed for networks that need to distribute extremely
precise and reliable time. It receives a time reference and distributes it to
other devices on the network using the protocols PTP and NTP.

---

#### Concept of PNT — Position, Navigation and Timing

For the case of the EdgeGM 7000, the most important component is time. The GNSS
normally provides a good time reference, but it is not always reliable. The PNT
can suffer from:

- Jamming: intentional external interference.
- Spoofing: sending false signals from attackers pretending to be a legitimate
  reference.
- Meaconing: a legitimate signal is captured, delayed, and retransmitted.

VIAVI uses the TrustedPNT technology that combines, authenticates, and qualifies
multiple timing sources.

In other words, in the hierarchy, the EdgeGM acts as a master orchestrating the
various timing references (GNSS / GEO / LEO).

---

#### NTP vs PTP

#### Network Time Protocol (NTP):

When we have a server NTP used to synchronize devices on the network generally,
and there is no need for extreme precision.

Normally used to synchronize:

- Servers
- PCs
- Applications
- Network equipment
- Operating systems

---

#### Precision Time Protocol (PTP):

It is used when we need a much more precise synchronization, and that's where
the EdgeGM comes to the top of the hierarchy and acts as a filter between the
other equipment on the network.

Note: I made some minor changes to the text to make it flow better in English,
but the original meaning and content are preserved.
