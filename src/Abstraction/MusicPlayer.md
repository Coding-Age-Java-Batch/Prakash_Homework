interface MusicPlayer {
void playSong(String name);
}
class SpotifyPlayer implements MusicPlayer {

    public void playSong(String name) {
        System.out.println("Spotify is playing: " + name);
    }

    public void pause() {
        System.out.println("Spotify playback paused.");
    }
}
class LocalPlayer implements MusicPlayer {

    public void playSong(String name) {
        System.out.println("Local Player is playing: " + name);
    }

    public void pause() {
        System.out.println("Local Player playback paused.");
    }
}

public class Main {
public static void main(String[] args) {

        SpotifyPlayer spotify = new SpotifyPlayer();
        LocalPlayer local = new LocalPlayer();

        spotify.playSong("Shape of You");
        spotify.pause();

        local.playSong("Believer");
        local.pause();
    }
}