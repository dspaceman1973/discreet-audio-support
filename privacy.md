  # Discreet Audio — Privacy Policy

  **Last updated: 17 May 2026**

  Discreet Audio is a multi-track audio recorder for macOS, developed by Danny McCullough. This privacy policy describes what data the app handles,
  where it goes, and what it doesn't do.

  ## Short version

  Discreet Audio doesn't collect, transmit, or share any personal data. Everything you record, every setting, every sound report stays on your Mac.
  No telemetry, no analytics, no third-party SDKs, no servers.

  ## Data we don't collect

  - **No personal information.** No name, email, phone number, address, account ID, device identifier, or location.
  - **No usage analytics.** We don't track which features you use, when, or how often.
  - **No crash reports** sent to us automatically. macOS may show its own crash reporter; that's between you and Apple.
  - **No advertising identifiers.** The app does not contain any ad SDKs.
  - **No third-party tracking.** The app does not include any third-party analytics, attribution, or marketing SDKs.

  ## Microphone access

  Discreet Audio requests access to your audio input devices (built-in microphone, USB audio interfaces, LTC sources, etc.) for the sole purpose of
  recording audio you initiate.

  Recorded audio is stored locally on your Mac, in a folder of your choosing. The app does not analyze, upload, or share recorded audio. It never
  sends audio anywhere off your machine on its own.

  ## Network access (in-app remote control)

  Discreet Audio includes an optional in-app remote-control feature that runs a local HTTP and WebSocket server on TCP port 7878.

  - The server is reachable **only on your local Wi-Fi or Ethernet network**.
  - Access is gated by a 4-digit pairing code you must enter in the in-app Remote Control dialog.
  - The web companion lets paired devices control transport, edit session metadata, mark circled takes, and listen to the operator's solo bus.
  - **No network traffic from the app ever leaves your local network.** The app does not connect to any external services or servers.

  You can simply ignore the remote-control feature if you don't want to use it; it consumes negligible resources.

  ## Data we store locally
  
  All app data is stored on your Mac in your sandbox container:

  ~/Library/Containers/com.beforeandaftersciencesound.discreetaudio/Data/

  This includes:
  
  - **Recorded audio** — in `Documents/DiscreetAudio/` by default, or any folder you've explicitly granted the app write access to via the system
  file picker.
  - **Settings** — `Library/Application Support/DiscreetAudio/preferences.xml`
  - **Take recovery file** — same folder, restores the last session if the app crashes mid-take.
  - **Remote pairing tokens** — `Library/Application Support/DiscreetAudio/remote_trust.json`. These authenticate previously-paired devices and never
   leave your machine.
  - **Remote server log** — `Library/Logs/DiscreetAudio/remote.log`. Local diagnostic only.

  You can inspect or delete any of this at any time via Finder. Uninstalling the app removes the container automatically.

  ## Folders outside the container

  If you point Discreet Audio's output folder at a location outside its sandbox container (e.g., `~/Music/Sessions/`), macOS prompts you with a file
  picker and the app stores a security-scoped bookmark so it can keep writing to that folder across launches. The bookmark is stored only on your
  Mac, in the settings file above.
  
  ## Children's privacy

  Discreet Audio is not directed at children. We do not knowingly collect any information from anyone, including children under 13.

  ## Third-party services
  
  Discreet Audio does not integrate with any third-party services, analytics platforms, or advertising networks.

  ## Changes to this policy

  If this policy ever changes, the updated version will be posted at the same URL. The "Last updated" date above will reflect the most recent
  revision. There's no third-party data-handling that could change behind the scenes — your data continues to never leave your Mac.

  ## Contact

  For questions about this policy, email dannymccullough@mac.com
