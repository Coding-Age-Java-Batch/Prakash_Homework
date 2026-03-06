interface Playable {
void play();
}

class MusicPlayer implements Playable {
public void play() {
System.out.println("Playing Music...");
}
}

class VideoPlayer implements Playable {
public void play() {
System.out.println("Playing Video...");
}
}

public class TestPlayable {
public static void main(String[] args) {

        Playable[] players = {
            new MusicPlayer(),
            new VideoPlayer()
        };

        for(Playable p : players)
            p.play();
    }
}