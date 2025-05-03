import java.util.Random;
/* Here's a random thing I generated out of pure annoyance with everything and Git not considering me a collaborator on a previous project. 
God I'm tired. */ 


public class QuotePrinter {
    public static void main(String[] args) {
        String[] lisbethQuotes = {
            "\"I don't have many friends. I don't trust people who easily make friends.\"",
            "\"No one else is going to save you. That’s just life, you have to save yourself.\"",
            "\"Everybody has secrets. It’s just a matter of finding out what they are.\"",
            "\"She was not a person who could be manipulated.\"",
            "\"I always assume people have secrets.\"",
            "\"People always have secrets. It's just a matter of finding out what they are.\"",
            "\"You know what's scary? That I can’t feel anything when I hurt people.\""
        };

        String[] rhiannonQuotes = {
            "\"I smile, but I’m dead behind the eyes.\"",
            "\"Sometimes I wonder if I’m a bad person pretending to be good, or a good person pretending to be bad.\"",
            "\"The world is full of hypocrites. I’m just more honest than most.\"",
            "\"Murder is just a stronger form of punctuation.\"",
            "\"I fake everything. Smiles, conversations, pleasantries. All of it.\"",
            "\"I’m not broken. I just prefer things my way.\"",
            "\"It’s not rage, it’s clarity. A pure moment of intention.\""
        };

        Random rand = new Random();
        boolean pickLisbeth = rand.nextBoolean();

        if (pickLisbeth) {
            int index = rand.nextInt(lisbethQuotes.length);
            System.out.println("Lisbeth Salander (The Girl with the Dragon Tattoo):");
            System.out.println(lisbethQuotes[index]);
        } else {
            int index = rand.nextInt(rhiannonQuotes.length);
            System.out.println("Rhiannon Lewis (Sweetpea):");
            System.out.println(rhiannonQuotes[index]);
        }
    }
}
