# Astra RoboCasa Planning & Recovery Replay

A successful GPT-6-Astra / xhigh **PanTransfer, seed 2** episode, recorded with HarnessVLA / RPent on RoboCasa365.

The task is to dump the vegetables from a pan onto a plate, then return the pan to the stove. Four initial VLA calls did not complete the task. The agent then used 44 analytic-control actions to grasp, carry, tilt, recover a slipped pan, return it to the stove, and withdraw. The environment confirmed success.

The viewer shows all 79 recorded tool calls and their arguments, results, camera snapshots, and the agent's contemporaneous public execution commentary. The original 115.55-second video contains 2311 frames at 20 fps; the full run took 1128.4 seconds. Inference and waiting time are not in the video. A button jumps directly to the agent takeover at 64 seconds.

Action alignment uses primitive step counts; the two composite grasp boundaries were recovered by matching returned camera images to the video. All 48 action-end frames were checked and the total matches the video frame count. Chapter labels are retrospective annotations, not VLA prompts.

Local machine paths are replaced with relative labels. This is a mixed VLA/agent episode, not a zero-VLA run or a controlled comparison against a VLA-only baseline.

Built on [RPent](https://github.com/RLinf/RPent), RoboCasa, and RLDX-1.
