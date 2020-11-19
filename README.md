# Xylophone
![Xylophone](image.png?raw=true "Xylophone")

* play audio 
```swift
import AVFoundation

var player: AVAudioPlayer!

func playSound(soundName: String) {
    let url = Bundle.main.url(forResource: soundName, withExtension: "wav")
    player = try! AVAudioPlayer(contentsOf: url!)
    player.play()
}
```

* Run code after a delay
```swift
  DispatchQueue.main.asyncAfter(deadline: .now() + 0.2 ) {
      // code to run after delay
  }
```
