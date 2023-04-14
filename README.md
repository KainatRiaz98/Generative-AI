# Stable Diffusion + Textual Inversion Embedding: The Winning Combination for Consistent Character Generation

Storytelling is an essential part of human culture, and characters play a crucial role in bringing narratives to life. However, creating visually appealing and consistent characters can be a challenging task, especially for artists and writers with limited resources. That's where advanced techniques like textual inversion embedding come in. By utilizing this cutting-edge approach, I have been able to generate consistent and visually stunning characters that are perfect for storytelling purposes.


In this blog post, I'll take you through the process of creating consistent characters using textual inversion embedding. I'll explain the concept of textual inversion embedding, how it works, and the benefits of using this technique for character generation. I'll also provide examples of the characters I have generated using this approach and how my clients have used them in their creative projects. So, whether you're an artist, writer, or simply interested in the latest advancements in character generation, read on to discover how textual inversion embedding can help you bring your creative visions to life.

## So, what is stable diffusion?

Stable Diffusion might sound like a fancy term from a chemistry lab, but it's actually a powerful technique used in image generation! It's a bit like a magic spell that allows us to create stunning and consistent images that are perfect for storytelling.

So, what is stable diffusion? In simple terms, it's a process of gradually modifying an image by adding noise to it over multiple steps. By doing this, we can generate a sequence of images that start from a random noise pattern and gradually morph into the desired final image.

Think of it like baking a cake. You start with raw ingredients, mix them together, and then put them in the oven to transform into a delicious treat. In stable diffusion, we start with a random noise pattern, apply some mathematical magic, and voila! We end up with a visually stunning image.

| ![1](https://user-images.githubusercontent.com/88194731/231697089-c75af90a-3822-41bb-b2d4-9511df7c7a17.PNG) |
|:--:| 
| *Images generated using stable diffusion* |

So, whether you're a fan of magic spells or baking cakes, stable diffusion is a powerful tool that can help you create stunning images for all sorts of creative projects. And when it comes to consistent character generation, it's a game-changer!

So, you want to create consistent characters that look amazing every time? Well, buckle up, because I'm about to take you on a wild ride through the magical world of textual inversion embedding and stable diffusion!
## Textual Inversion
First, let's talk about textual inversion embedding. It's like creating a whole new language just for image generation! By describing concepts in a new "language" using pre-trained text-to-image models, we can generate specific objects or styles that are unique and visually stunning.

| ![Capture](https://user-images.githubusercontent.com/88194731/231663954-3e83dd94-85b4-4cff-b5a1-0c8ee064df54.PNG) |
|:--:| 
| *An example of textual inversion* |

I used stable diffusion to generate images of our character. It's like taking a blurry photo and turning it into a crystal-clear masterpiece! With hundreds of permutations to choose from, we can select the best images to use for later training.

Now, here's where things get really interesting. We start by generating 400 images of our character from different angles and focuses.


### Settings:

|*Prompt: An extreme closeup front shot photo of a beautiful 25yo Scotland woman (freckled face_1.2) with defined cheekbones, a straight nose, full lips, hazel eyes, chin dimple, square jaw, plucked eyebrows, red curly long hair, (neutral gray background:1.3), neutral face expression*|

|*Negative Prompt: (gray hair:1.3), (glasses:1.2), (earrings:1.2), (necklace:1.2), (high heels:1.2), young, loli, teen, child, (deformed, distorted, disfigured:1.3), poorly drawn, bad anatomy, wrong anatomy, extra limb, missing limb, floating limbs, (mutated hands and fingers:1.4), disconnected limbs, mutation, mutated, ugly, disgusting, blurry, amputation, tattoo*|

Sampling method: DPM++ 2M Karras
Sampling steps: 30
Restore Faces: On
Tiling: Off
Hires. fix: Off
Width: 512
Height: 512
CFG Scale: 7
Seed: -1

Now let's spice up your character variations with some different angles and zoom levels! Head to the Script menu and select X/Y/Z Plot. In X values, copy and paste these five zoom levels:

extreme closeup, medium closeup, closeup, medium shot, and full body

This will give you images of your character from different distances. In Y values, copy and paste these five viewing angles:

front shot, rear angle, side angle, shot from above, and low angle shot.

Now that you've told the AI to generate 25 different versions of your character to choose from for training. Make sure to check "Keep -1 for seeds" and set Batch Count and Batch Size to 4 (or 2 and 8 if your GPU is feeling feisty). Let the AI work its magic and generate 16 images for every permutation of angles and zoom levels. Your character is about to become the most versatile one out there!

It's time to name our character for the tagging - we'll call her 3m1ly. Make sure the name is unique, so we can train the AI to recognize her specifically. Keep it short and sweet - just one word, without any spaces. We don't want the AI getting confused with other tokens that already have a meaning.

![xyz_grid-0000-997563325-an extreme closeup front shot photo of a beautiful 25yo Scotland woman (freckled face_1 2) with defined cheekbones, a straight n, ](https://user-images.githubusercontent.com/88194731/231701063-72fde37c-98ea-48bb-91f5-24fcf83bcb11.jpg)

 But not all of them make the cut. We filter out the images until we're left with about 25 images that look almost identical and have the same background.
 
 
But wait, there's more! We carefully craft the caption to not include the things we want our model to learn, like the character's facial features and personality traits. We only include the background and clothes because we don't want our model to learn those things and always generate our character in same outfit and background. 

In the end, we're left with a set of consistently stunning characters that are ready to bring your stories to life.

## Results

Meet Emily, Emily is a natural beauty, with her striking red curls and high cheekbones. Her Swedish heritage is evident in her fair skin and bright blue eyes, and her warm smile lights up any room. It's no wonder she's such a beloved member of her community.

|![Untitled drawing](https://user-images.githubusercontent.com/88194731/231721558-545b72f2-c406-4ee9-aa97-4af1c4eb1924.jpg) |
|:--:| 
| *the Swedish beauty with red curls and cheekbones that could cut glass. She's a force to be reckoned with!* |

Emily is a master in the kitchen, whipping up delicious meals with ease. Her Swedish heritage has influenced her cooking style, and she loves experimenting with new flavors and ingredients. Here she is, preparing her signature dish passed down from her grandmother.


| ![Untitled drawing (2)](https://user-images.githubusercontent.com/88194731/231733644-818d6f01-fcef-4901-8c28-b05f7c190e04.png) |
|:--:| 
| *Looks like Emily is cooking up a storm! Who's hungry?* |
When Emily isn't cooking up a storm in the kitchen, you can find her tending to her garden. She has a green thumb and a love for all things botanical. Here she is, surrounded by her beautiful flowers and plants, enjoying a peaceful moment in nature.

| ![Untitled drawinghj](https://user-images.githubusercontent.com/88194731/231738704-d14e8243-da17-482c-81e1-fe2d7de388a2.png) |
|:--:| 
| *Emily has quite the green thumb! Who knew gardening could look so chic?* |


Not only is Emily talented in the kitchen and garden, but she's also a gifted musician. She leads a local choir, helping them to perfect their harmonies and reach new heights with their performances. Here she is, conducting a practice session with her choir members, bringing beautiful music to life.


|![Untitled drawing (1)](https://user-images.githubusercontent.com/88194731/231733630-7aadb325-f2ae-47a9-acea-5c22fe0e0333.png) |
|:--:| 
| *Emily knows how to bring harmony to a group of people - both in music and in life.* |

## Conclusion

Creating consistent and visually appealing characters is essential for storytelling purposes. And with the use of stable diffusion and textual inversion embedding, it is now easier than ever before to generate these characters. As we have seen, this technique can be used to create a wide variety of characters, from Swedish beauties like Emily to astronauts building castles on Mars.

But the applications of this technique don't stop there. Imagine using consistent character generation to create characters for video games, comics, and movies. With this technique, you could quickly generate hundreds of unique characters and bring them to life in engaging and exciting ways.

Or how about using this technique for virtual reality experiences, where users could interact with lifelike characters in immersive environments? The possibilities are endless, and I can't wait to see how this technique will continue to shape the future of character generation.

In conclusion, consistent character generation is a game-changer for creators and storytellers alike. With the use of stable diffusion and textual inversion embedding, we can now generate visually appealing characters that are consistent with our creative vision. So let's embrace this technique and unleash our creative potential!
