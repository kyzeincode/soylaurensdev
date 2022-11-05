     						Hola , 👋 Soy Laurens!
```js
 public class YoSoyLaurensDev extends Humano implements Gamer, Desarrollador {

	@Override
	public String getName() {
		return "Laurens";
	}
	
	@Override
	public List<String> getAliases() {
		return Arrays.asList("soylaurensdev", "Mi Nombre");
	}

        public Laurens() {

        this.addLanguage("Java", "Javascript", "Python", "C#", "C++");
     }
   }

	@Override
	public String aboutme() {
		return "Me gusta jugar Minecraft " +
		"\n" + "Me gusta programar en Java";
	}
    
	@Override
	public void codingStuff() {
		String[] learning = ["Java", "Node.js / Discord.js", "Python", "C#", "C++"];
		String tryingTo = "Programar lo mejor posible en clientes/plugins/mods de Minecraft y bots de discord";
	}
	
} 


public abstract class Humano {

  @Getter private final String username;
  @Getter private final String country;

  private Set<String> languages = new HashSet<>();
  private Set<String> experiences = new HashSet<>();

  public Humano(String username, String placeilive) {
      this.name = username;
      this.country = placeilive;
  }

  public void addLanguage(String... language) {
      this.languages.addAll(language);
  }
  
}
```
