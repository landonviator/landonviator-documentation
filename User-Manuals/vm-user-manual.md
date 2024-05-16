# Vibe Mechanic Mk II

Thank you so much for downloading Vibe Mechanic Mk II!

This plugin is a ground-up re-design of my Vibe Mechanic plugin released back in 2021. This new plugin adds quite a few awesome features, such as the ability to re-order the effect modules, mid-side processing, and carefully crafted and recorded impulse responses of real hardware.

Let's get into it!

## Modules Overview

VM (Vibe Mechanic) contains four effects modules in the style of rack-mounted hardware. You've got a Distortion, Tone, Effects, and Space module, each of which can be moved and dragged around the interface to re-order like other rack-mount-style plugins out in the market.  

To re-order the rack, simply place the mouse cursor on an area of the module not taken up by a gui control (like a button or slider), then click and drag to any other rack space.

You can also see that each module has two buttons at the top called "M" and "S". These are mute and solo buttons for each module.

### Distortion Module

The Distortion Module serves as the initial stage in our audio plugin's default processing chain, offering two distinct engines to shape your sound with various forms of distortion.

Upon accessing the distortion module, you are greeted with a dropdown menu that allows you to choose the type of distortion. It's important to note that our module is equipped with two separate distortion engines, each with its own unique controls and characteristics.

#### Distortion Engine One - Bit Crusher

The first engine is designed as a Bit Crusher, ideal for achieving those sought-after lo-fi effects. It operates with three specific controls:

`Resample`: Adjusts the audio downsampling rate, crucial for obtaining the classic bit crusher effect. <br>
`Depth`: Modifies the bit depth of the audio, enabling you to explore a range of noisy textures.<br>
`Noise`: Controls the volume of an integrated noise generator, adding an additional layer of texture to your sound.

Please note, the Drive and Mix controls do not influence this engine; they are reserved for the second distortion engine.

#### Distortion Engine Two - Saturator

Our second engine offers a more conventional saturation distortion, celebrated for its musicality and warmth. It utilizes two main controls:

`Drive`: Regulates the amount of signal fed into the distortion, allowing for a gradual increase in saturation as the input gain is raised. <br>
`Mix`: Enables you to blend the processed signal with the original, unprocessed audio, ensuring flexible manipulation of the distortion effect. <br>

**Filtering and Signal Flow**

Following the distortion engines, the module features two filters for fine-tuning the tonal characteristics of the distorted signal:

`HP Filter`: Adjusts the cutoff frequency of a high-pass filter, applied after the second distortion engine to sculpt the higher frequencies. <br>
`LP Filter`: Sets the cutoff frequency of a low-pass filter, also placed after the second distortion engine, for control over the lower frequencies.

The signal chain within the distortion module flows as follows: 

**Bit Crusher -> Distortion -> Filters**

This configuration offers a comprehensive suite of tools for crafting your desired distortion effects, paving the way for further processing in subsequent modules of the plugin.

### Tone Module

The Tone Module is your comprehensive tool for shaping timbre and color in your audio projects. It features an IR menu, which offers a selection of five impulse responses captured from diverse real-world speakers, providing you with a range of sonic textures. Additionally, the module includes a Telephone Effect section that simulates the distinct sound of a telephone speaker, which is popular in many lofi songs. For precise adjustments, utilize the six-band graphic EQ to fine-tune your audio to perfection.

### Speaker Model

The IR menu features five unique impulse responses, each meticulously recorded from authentic real-world speakers. Below is a list of the available models:

`Japanese lofi 1975` - Captured from a Japanese-made cassette recorder circa 1975, this impulse response delivers a characteristic lo-fi, slightly distorted sound.

`Sweet 80's Tape` - Derived from a popular stereo cassette recorder of the 1980s, this model offers a pleasing enhancement to the high-end frequencies.

`Smart Phone Speaker` - An impulse response directly recorded from a modern smartphone speaker.

`Ear Buds` - This IR is taken from wired earbuds commonly included with contemporary smartphones.

`Cheap Intercom` - An impulse response from an economical $20 intercom system, sourced from an online retailer.

#### Phone Effect

Achieve the iconic telephone vocal effect favored in lo-fi music with this dedicated section. Instead of using impulse responses (IRs), it employs filters to create the distinctive sound. This approach offers you the flexibility to either enhance the output from the IR section or use the Telephone Vocal Effect on its own for a standalone impact. The parameters are listed below:

`Range` - Adjusts the width of the frequency range allowed through. A narrower range intensifies the lo-fi characteristic of the sound.

`Center` - Sets the central frequency of focus for the range. Moving this slider changes the specific area of frequency filtering.

`Resonance` - Modifies the resonance level at the center frequency. Increasing this value enhances feedback and resonant effects.

`Mix` - Controls the blend of the telephone model effect with the original signal.

#### EQ

This six-band EQ provides additional control for shaping your sound. Use the sliders to adjust the gain for each frequency band.

The cutoff frequencies from lowest to highest are `15 Hz`, `125 Hz`, `500 Hz`, `2000 Hz`, `5000 Hz`, and `19000` Hz.

### Effects Module

The Effects Module offers a variety of pitch and modulation effects, including models for pitch drift (wow and flutter), chorus, and tremolo. These effects are designed to infuse your tracks with additional vibe and character.

#### Tape Wow and Flutter

`Wow Rate` - This control adjusts the frequency or speed at which the pitch of the audio signal deviates from its original pitch. This deviation is referred to as "detuning." The rate setting determines how quickly these pitch variations occur over time. A lower setting results in slower, more gradual pitch changes, which can subtly alter the tonal quality of the sound, giving it a gently warbling effect. Increasing the rate results in faster, more frequent pitch shifts, producing a more noticeable and dramatic vibrato-like effect.

`Flutter %` - This control sets the likelihood or probability of the Flutter effect being applied to the audio signal. Flutter is a rapid, small-scale variation in the pitch of the sound, often mimicking the irregularities found in old tape recordings or vinyl records. The percentage value you select determines how often these pitch variations will occur during playback. Higher percentages increase the frequency of these occurrences, making the flutter effect more pronounced and noticeable. 

`Wow Depth` - Adjusts the intensity of the Wow effect, determining how pronounced it is.

`Flutter Depth` - Modifies the intensity of the Flutter effect, defining how deep the effect is.

#### Chorus

`Rate` - This control adjusts the speed at which the chorus effect modulates. Modulation refers to the periodic variation in some aspect of the sound, in this case, pitch. A higher rate will cause the pitch variations to occur more quickly, creating a more pronounced wobble effect.

`Depth` - Sets the intensity of the modulation applied by the chorus effect.

`Mix` - Determines the balance between the original, unprocessed signal and the processed signal with the chorus effect.

#### Tremolo

`Rate` - This control adjusts the speed of the tremolo effect by setting the note division relative to your DAW's tempo. The tremolo effect rhythmically modulates the volume of the sound to create a pulsating effect. The available rate options allow you to synchronize the tremolo with your track's tempo, offering divisions such as quarter note, eighth note, triplet, sixteenth note, dotted eighth note, and sixtuplet (sixteenth note triplet). Choose a division to define how quickly or slowly the volume fluctuations occur in relation to the beat of your music.

`Depth` - This control determines the extent of the volume modulation applied by the tremolo effect. The depth setting adjusts how dramatic the volume changes are, ranging from subtle fluctuations to full pulsations. At its maximum setting (1), the tremolo effect can vary the volume from complete silence to full loudness, providing a pronounced and dynamic audio experience. Lower settings result in more gentle variations, allowing for a more nuanced modulation effect.

### Space 

The Space Module enhances your tracks with reverb and delay effects, essential tools for creating the illusion of space within your music. These effects can simulate environments from small rooms to vast landscapes, adding depth and dimension to your audio.

#### Reverb

A lush, lightweight algorithmic reverb that's designed for ease of use and quick adjustments. It creates a rich and immersive atmosphere without overburdening your system, making it ideal for any mixing scenario.

`Size` - Adjusts the scale of the virtual room simulated by the reverb. Increasing the size expands the room, enhancing the reverb's tail and making the space feel larger and more open.

`Damping` - Controls the reverb's damping, which affects the brightness of the sound. Higher damping settings reduce high frequencies, resulting in a warmer and more muffled reverb effect.

`Width` - Sets the stereo width of the reverb, allowing you to fine-tune the spatial distribution between mono and full stereo. This control can enhance the listener's sense of space and placement within the mix.

`Mix` - Manages the balance between the wet (effected) and dry (uneffected) signals. This control is crucial for blending the reverb naturally with your original track, from subtle ambience to profound reverberation.

#### Delay

Experience the classic charm of a simple, analog-inspired delay effect designed to enrich your tracks with rhythmic echoes. This effect mimics the behavior of traditional analog hardware, providing warmth and depth.

`Time` - Similar to the tremolo, the delay time is automatically synced to your DAW's tempo. This synchronization ensures that the echo effect seamlessly integrates with your music's rhythm. The delay offers various rate options to match the track’s tempo, including divisions such as quarter note, eighth note, triplet, sixteenth note, dotted eighth note, and sixtuplet (sixteenth note triplet). 

`Feedback` - This control adjusts the feedback level of the delay effect. Increasing the feedback causes the echoes to repeat more frequently, extending the tail of the delay and intensifying the effect. High feedback settings can create a cascading series of echoes, adding complexity to your sound.

`Tone` - Manages the tone of the delay by adjusting the cutoff frequency of a low-pass filter applied to the delayed signal. This allows you to control the brightness of the echoes, making them crisper or more subdued based on your preference.

`Mix` - Controls the mix between the wet (processed) and dry (original) signals. This balance is crucial for achieving the desired prominence of the delay effect, from subtly enhancing the track’s texture to creating prominent, rhythmic patterns.

#### IO

`Input` and `Output` volume. Located on the left side of the interface, you will find a slider dedicated to adjusting the gain of the signal entering the plugin. This control is crucial for setting the initial signal level to ensure optimal processing. On the right side of the interface, another slider adjusts the gain of the signal exiting the plugin. This allows for precise gain staging, facilitating seamless integration with other plugins in your signal chain, ensuring levels are matched and distortion is minimized.

### Header Panel

At the top of the interface, you'll find the header panel with lots of helpful features, such as the `A/B preset`,  `preset browser`, `oversampling menu`, and `stereo menu`.

#### A/B Preset

The A/B preset function facilitates effortless switching between two distinct local presets. This feature is designed to simplify the process of comparing different settings or states of your audio adjustments. By toggling between Preset A and Preset B, you can quickly evaluate and contrast the auditory impacts of various configurations without the need to manually adjust settings back and forth. This is particularly useful during mixing and mastering sessions where precise sound shaping is crucial, allowing you to make informed decisions on which settings best suit your audio material.

Using the A/B preset function is straightforward. When you select either Preset A or Preset B, the corresponding local preset is applied to the controls. From that point on, any adjustments you make to the controls will be automatically saved to the currently selected preset. Initially, when you select Preset A or B for the first time, you may notice that the controls do not change positions; this is because they are set to their default states. This design ensures that you start from a known, stable configuration each time you switch between presets, allowing for consistent modifications and comparisons.

#### Preset Browser

The preset browser offers a user-friendly interface for saving your custom presets and accessing a variety of factory-made presets. All presets are saved in the .xml format within your documents directory, facilitating easy sharing with friends or clients who can load these presets into their own Vibe Mechanic plugin. Additionally, the browser includes a rich selection of factory presets, carefully crafted by myself and other talented creators, providing a wide range of starting points for your sound design.

#### Oversampling Menu

The Oversampling menu in Vibe Mechanic provides options to enhance the audio quality by selecting different oversampling factors. You can choose from two, four, or eight times oversampling rates. Oversampling reduces digital distortion and aliasing effects, which are common when processing high frequencies.

#### Stereo Menu

The Stereo menu provides versatile options for managing the stereo field of your audio tracks. You can choose to process audio in full stereo, preserving the spatial distribution between the left and right channels. Alternatively, you can sum the stereo signal down to mono, which combines both channels into a single, centered audio track. This is particularly useful for ensuring compatibility across various playback systems or for focusing the listener's attention. Additionally, the menu offers the option to process only the mid (mono) channel or only the sides (stereo difference) of the signal. Processing only the mid channel emphasizes elements like vocals and bass that are typically centered in a mix, while processing only the sides enhances the ambient and spatial effects located primarily in the stereo field. This flexibility allows for creative control and precise manipulation of your audio's spatial characteristics.
