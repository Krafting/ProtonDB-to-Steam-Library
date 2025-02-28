
```bash
This build add the Native categorie to the Original script (all credits to CorruptComputer on GitHub!)
```

# ProtonDB to Steam Library [![Build Status](https://travis-ci.com/CorruptComputer/ProtonDB-to-Steam-Library.svg?branch=master)](https://travis-ci.com/CorruptComputer/ProtonDB-to-Steam-Library)[<img src="https://discordapp.com/assets/f8389ca1a741a115313bede9ac02e2c0.svg" width="45" height="45" alt="ProtonDB Discord" title="ProtonDB Discord">](https://discord.gg/uuwK9EV)

This is just a small python script to pull ratings from ProtonDB and import them into your Steam library as tags.

Here is a screenshot which shows how it looks once ran:

![Screenshot](screenshot.png)

### Dependencies

You'll need to install [vdf](https://github.com/ValvePython/vdf) before this can run. 
You can install it via pip with: 
```bash
pip install vdf
```

### Running

**WARNING:** This may clear all of your current tags in Steam. You have been warned!

This can be simply run with: 
```bash
python ProtonDB-to-Steam-Library.py
```

It will also ask before saving the file, so if you want to just test it out theres no real danger of overwriting anything.

You can also specify a custom path to your sharedconfig.vdf with: 
```bash
python ProtonDB-to-Steam-Library.py -s /path/to/sharedconfig.vdf
```

The full command line options can be viewed with: 
```bash
python ProtonDB-to-Steam-Library.py -h
```

### Contributing

If you run into any issues please attach the output from the script to your issue, along with the sharedconfig.vdf file which was selected.

All feedback is welcome and appreciated! Please make an issue if you have any ideas or feedback, I would love to hear them!

If you would like to make a PR all I ask is that you are also open to feedback on your written code.

### Troubleshooting

If you are finding that only some of your Proton compatible games are being categorized try this:

1. Select all of the games in your library
2. Right click -> Set Categories...
3. Add some random category to them all (you can remove this later)
4. Close Steam to force it to write all of your games to the sharedconfig.vdf file
5. Try running the script again

If anything is still not working you can open an issue here, or join the ProtonDB Discord server (link is at the top of this README).
Questions regarding this tool can be asked in #protondb-discussion or in #off-topic. Please respect the rules of the server if you join!
