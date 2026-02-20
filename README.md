# KEYGRAVE TELEMETRY

**Beta Enrollment — A Chasm Logic QA Initiative**

Keygrave Telemetry parses your Claude Code session history and generates a compatibility assessment for the [CCK-3 Approval Peripheral](https://qry.zone/fun/claudetite-keyz/). The tool analyzes your keypress patterns, approval-to-rejection ratios, and time-to-decision metrics to determine whether you are suitable for hardware-accelerated approval workflows.

Results are presented as a standardized telemetry report. Your Beta Tester number is assigned at enrollment.

---

## Install

```bash
curl -sL https://raw.githubusercontent.com/qry/keygrave/main/keygrave -o keygrave && chmod +x keygrave
```

Or clone this repository:

```bash
git clone https://github.com/qry/keygrave.git
cd keygrave
chmod +x keygrave
```

## Usage

```bash
./keygrave          # Enrollment + report (first run)
./keygrave report   # Generate telemetry report
./keygrave enroll   # View enrollment terms
./keygrave status   # Data inventory
./keygrave version  # Version + credits
```

## Sample Output

```
┌───────────────────────────────────────────────┐
│  KEYGRAVE TELEMETRY — SESSION REPORT          │
│  Beta Tester #0847                            │
├───────────────────────────────────────────────┤
│                                               │
│  Approvals                               412  │
│    (tool accepts)                        401  │
│    (typed)                                11  │
│  Rejections                                3  │
│  Key 3 Presses                             0  │
│  Avg. Time to Approval                  0.4s  │
│  Longest Hesitation                     1.1s  │
│  Diffs Reviewed                      UNKNOWN  │
│                                               │
│  CCK-3 Compatibility                  99.3%   │
│                                               │
│  Assessment: YOUR KEYBOARD HAS 101           │
│  UNNECESSARY KEYS.                            │
│                                               │
├───────────────────────────────────────────────┤
│  You are the product.                         │
│  Thank you for your participation.            │
│  This data has not been transmitted.¹         │
│                                               │
│  ¹ That you know of.                          │
└───────────────────────────────────────────────┘
```

## Enrollment Terms (Abbreviated)

By running this tool, you acknowledge that your approval patterns constitute biometric data under the Chasm Logic Participant Agreement (Rev. 4.1). You surrender all claims to originality regarding your keypress sequences. Pressing "1" is not a creative act. You do not own it.

Full terms are presented at enrollment. You will be asked to press 1 to proceed. This is not ironic.

## The Daemon

The telemetry agent runs as a background daemon.

This is not that kind of demon. It is watching you.

## Privacy

This tool runs locally. It reads `~/.claude/` and prints numbers to your terminal. Nothing is transmitted, collected, or shared. There are no network calls. There is no tracking. There is no telemetry server. The "telemetry" is the joke. The numbers are real.

See [PRIVACY.md](PRIVACY.md) for the unembellished version.

## Requirements

- Bash 4+
- Standard Unix tools (grep, awk, find, date)
- Claude Code session data at `~/.claude/`

## Related

- [CCK-3 Product Page](https://qry.zone/fun/claudetite-keyz/) — The approval peripheral
- [QA Incident Report](https://qry.zone/fun/chasm-logic/qa/) — Testing documentation
- [Ultra Wristband Brief](https://qry.zone/fun/chasm-logic/wristband/) — Commitment hardware

---

<sub>Compiled by J. Reeves, Communications Division. Corrections to this document have been submitted. They were rejected via Key 1.</sub>
