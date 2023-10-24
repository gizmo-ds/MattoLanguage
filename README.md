# MattoLanguage 🤡

[![爱发电](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fafdian.net%2Fapi%2Fuser%2Fget-profile%3Fuser_id%3D75e549844b5111ed8df552540025c377&query=%24.data.user.name&label=%E7%88%B1%E5%8F%91%E7%94%B5&color=%23946ce6)](https://afdian.net/a/gizmo)
[![License](https://img.shields.io/github/license/gizmo-ds/MattoLanguage?style=flat-square)](./LICENSE)

MattoLanguage is a brand-new programming language, shining with a unique 🤡 style, designed to provide developers with an absolutely enjoyable coding experience. This language is built on a foundation of modern syntax and cheekily incorporates the strengths of other contemporary programming languages, making programming feel like dancing at a wild coding party.

## 🕊️ Features (still in the works, don't rush us)

- **Modern Syntax**: MattoLanguage adopts the cool syntax elements of modern programming languages to offer you a clear, intuitive, and highly entertaining way to code.

- **Decently Useful Type Inference**: MattoLanguage will introduce type inference to reduce those tedious type declarations, allowing you to write code with ease, as if you were in the midst of a grand celebration of development.

- **Even More Advanced File Extension**: Our file extension is `.🤡` because we know we're more advanced than [🔥](https://www.modular.com/mojo)!

[![asciicast](https://asciinema.org/a/616729.svg)](https://asciinema.org/a/616729)

> "🤡" better than "🔥" —— [Node.js v18.16.0](https://nodejs.org/download/release/v18.16.0/)

## 💡 Examples

<details>

```🤡
// hello.🤡
mod main

const (
	std = import("std")
	println = std.log.println
	$f = std.fmt.$f
)

const (
	default_country = "Bolivia"
	default_age: u32 = 20
	default_gender = Gender.pizza
)

pub enum Gender {
	male = "male"
	female = "female"
	pizza = "pizza"
	banana = "banana"
	other = "other"
}

class Human {
	pub name: string
	age: u32
	pun mut gender: Gender
	married: bool = false
	pub mut country: string

	Human(<name, <age, .{<married, <country = default_country})

	pub fn i_am() string {
		f"I am {.name}"
	}

	defer fn die() {
		println(f"{.name} say: Oh, I'm dead 💀")
	}
}

pub fn say_hello(name: string, age:u32) {
	const a_human = new Human(name, age)
	println(f"{a_human.name} say: Hello, {a_human.i_am()} ✨")
}

fn main(args: []string) {
	if (args.len() < 2) return println("🤔")

	for (args[1:]) |name, index| {
		say_hello(name, default_age + index)
	}
}

/*
./hello Alice Bob
Alice say: Hello, I am Alice ✨
Alice say: Oh, I'm dead 💀
Bob say: Hello, I am Bob ✨
Bob say: Oh, I'm dead 💀
*/
```

```🤡
// multiline_string.🤡
mod main

const std = import("std")

use string.{trim_space, dedent}

fn main() {
	const println = std.log.println
	const $html = std.fmt.$f

	const name = "Mom"
	const html_content = html`
		<div>
			<p>Hi {name}</p>
		</div>
	`.dedent().trim_space()
	println(html_content)
}

/*
./multiline_string
<div>
	<p>Hi {name}</p>
</div>
*/
```

</details>

## 🤝 Credits

MattoLanguage draws inspiration from the syntax of the following programming languages:

- [Go](https://golang.org/)
- [Zig](https://ziglang.org/)
- [🦀](https://www.rust-lang.org/ "I don't want to be prosecuted")

## ❤️ Sponsors

[![Sponsors](https://afdian-connect.deno.dev/sponsor.svg)](https://afdian.net/a/gizmo)

## ⚠️ Contact

Feel free to reach out to us on Twitter: [@gizmo_ds](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
