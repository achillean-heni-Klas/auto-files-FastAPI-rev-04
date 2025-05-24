
# **nestedform Kit**

![Python](https://img.shields.io/badge/python-3.12-blue)
![Raspberry Pi](https://img.shields.io/badge/pi-compatible-red)
![License: MIT](https://img.shields.io/badge/license-MIT-green)

> **Educational platform for classrooms.**

---

### About

nestedform is a teaching kit for middle-school using Python.
Simulates wheels, sensors, and actuators on low-cost hardware or browser emulator.

**Website:** [nestedformproject.io](https://nestedformproject.io)
**Docs:** [docs.nestedformproject.io](https://docs.nestedformproject.io)

---

###  Concept

Each "bot" is a YAML config + Python behavior:

```yaml
bot:
  name: explorer
  sensors: [ultrasonic, gyro]
  actuators: [motor, servo]
```

```python
def loop(bot):
    if bot.distance() < 10:
        bot.turn(90)
    else:
        bot.forward(1)
```

---

###  Try in browser

```
python3 -m nestedform.sim --map=basic
```

then open → `http://localhost:8080`

---

###  Components

* Cross-platform simulator (Pi, Linux, Web)
* Sensor emulation plugins
* Replay with camera overlay
* Curriculum JSON export

---

###  Roadmap

* [x] Web UI
* [ ] Visual programming
* [ ] Cloud sync

MIT License © [nestedformproject.io](https://nestedformproject.io)
