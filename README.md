# vertex_alt_metacity with border dark

vertex_alt_metacity

Edge theme modification vertex_alt_metacity with its dark edge and not the typical clear style

/usr/share/themes/Vertex_alt_metacity/metacity-1/metacity-theme-3.xml

I like this topic because it eliminates the title bar when maximizing the window, something that in the other themes I could not find, but its title bar loses color when using a dark theme, so these changes can enjoy a title bar dark with your dark theme.
These colors are not compatible with clear themes, only with dark themes, for this you have to search for the ideal color using a color palette and change them in the lines that you modify.

good luck xD

file metacity-theme-3.xml

# lines orginals of the file metacity-theme-3.xml

### title bar 

lines 13 - 21
```xml
13 <constant name="C_border_focused" value="gtk:custom(wm_border,#6d6d6d)" />
14 <constant name="C_border_unfocused" value="gtk:custom(wm_border,#6d6d6d)" />
15 <constant name="C_title_focused" value="gtk:custom(wm_title,#3c3c3e)" />
16 <constant name="C_title_focused_hilight" value="gtk:custom(wm_title_highlight,#ffffff)" />
17 <constant name="C_title_focused_hilight_dark" value="gtk:custom(wm_title_highlight_dark,#f7f7f7)" />
18 <constant name="C_title_unfocused" value="gtk:custom(wm_unfocused_title,#868686)" />
19 <constant name="C_titlebar_bg_a" value="gtk:custom(metacity_bg_a,#f7f7f7)" />
20 <constant name="C_titlebar_bg_b" value="gtk:custom(metacity_bg_b,#f3f3f5)" />
21 <constant name="C_titlebar_bg_highlight" value="shade/gtk:custom(metacity_bg_a,#f7f7f7)/1.4" />
```

### line maximized

lines 198 - 204
```xml
198 <draw_ops name="titlebar_max">
199		<gradient type="vertical" x="0" y="1" width="width" height="height">
200			<color value="shade/gtk:custom(metacity_bg_a,#f7f7f7)/0.95" />
201			<color value="C_titlebar_bg_b" />
202		</gradient>
203		<tint color="C_titlebar_bg_highlight" alpha="1.0" x="0" y="0" width="width" height="1"/>
204 </draw_ops>
```



-----------------------------------------------------------------------------------------

# modified lines of the file metacity-theme-3.xml
the changes are in the colors,
so that it looks like the attached image

### title bar modified

changes in lines 16, 17, 19, 20, 21
```xml
13 <constant name="C_border_focused" value="gtk:custom(wm_border,#6d6d6d)" />
14 <constant name="C_border_unfocused" value="gtk:custom(wm_border,#6d6d6d)" />
15 <constant name="C_title_focused" value="gtk:custom(wm_title,#3c3c3e)" />
16 <constant name="C_title_focused_hilight" value="gtk:custom(wm_title_highlight,#383838)" />
17 <constant name="C_title_focused_hilight_dark" value="gtk:custom(wm_title_highlight_dark,#383838)" />
18 <constant name="C_title_unfocused" value="gtk:custom(wm_unfocused_title,#868686)" />
19 <constant name="C_titlebar_bg_a" value="gtk:custom(metacity_bg_a,#404040)" />
20 <constant name="C_titlebar_bg_b" value="gtk:custom(metacity_bg_b,#404040)" />
21 <constant name="C_titlebar_bg_highlight" value="shade/gtk:custom(metacity_bg_a,#404040)/1.4" />
```

### line maximized modified

change in line 200
```xml
198 <draw_ops name="titlebar_max">
199		<gradient type="vertical" x="0" y="1" width="width" height="height">
200			<color value="shade/gtk:custom(metacity_bg_a,#5D5D5D)/0.95" />
201			<color value="C_titlebar_bg_b" />
202		</gradient>
203		<tint color="C_titlebar_bg_highlight" alpha="1.0" x="0" y="0" width="width" height="1"/>
204 </draw_ops>
```
