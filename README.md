# My-Mac-Terminal-Customs
This repo contains a read-me breakdown and other files for the customization of my Mac M2 terminal

### Using The Starship Preset
Starship's configurations live in a toml file in the `~/.config/starship.toml` file to be precise, this contains, by default the default starship setups right after running the `eval "$(starship init zsh)"` command the terminal changes and sets to the default starship configuration, or rather sets to whatever is configured in the toml file. 
That being said, starship has a set of Preset configurations, as toml files, available on the website for off-the-shelf usage; this means, if you feel like the default configuration right after installing starship is not your thing, or your taste ... -- whatever you call that; and you do not have time to configure by yourself either, then using another option already ready can be a much fair deal for you.
And that is where the Starship Presets come from, which you can find [here](https://starship.rs/presets/), there you will have a quite some configurations to choose from, but for me I decided to go with the [Pastel Powerline Preset] (https://starship.rs/presets/pastel-powerline.html), which I can not say it's like the best of all terminal configurations out there, but heey, I wanted from the biggining to go with the [P10K] (https://github.com/romkatv/powerlevel10k) configuration, and well the Pastel Power Line came out close, at least until I get to customize and make it to my best tastes (which I'll come back to next), that should do just fine.

Now how do we add make the Preset available in the terminal anyways??
Well, I'm glad you asked -- to do that, you need to run a couple, we, one command,
Remember the toml file that contains the configurations that get to be set in the terminal?
Well, yeah, you just need to edit the contents inside that file with your prefered preset contents, and that should be it, and to edit that you can use your favorite text editor, like `vim` in my case :) and paste the contents of the preset's toml file inside by running: `vi ~/.config/starship.toml` and then paste your toml contents there, and voila!
Or well, almost. Cause I know you're like, that's the command?
No, that is not the command, unless you decide to do it manually, but you don't have to cause the folks at Starship have put together a command to run that will do the job for you, in my case for the Pastel Power Line preset, the command I had to run was 
`starship preset pastel-powerline -o ~/.config/starship.toml
`

Which as you could guess, does the magic of editing the toml config file and write inside the Pastel (will keep it short like that)'s toml contents for you, so you don't have to do it manually.
