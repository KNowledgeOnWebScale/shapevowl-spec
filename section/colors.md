# Colors

## General

<table id="tab-general-colors">
  <tr>
    <th>Abstract Color Name</th>
    <th colspan="2">Concrete Color Recommendation</th>
    <th>Description</th>
    <th>Application</th>
  </tr>
  <tr>
    <td class="side">canvas</td>
    <td>#ffffff</td>
    <td>white</td>
    <td>Bright color with a good contrast to all other colors.</td>
    <td>canvas where are all other graph elements are shown on</td>
  </tr>
  <tr>
    <td class="side">foreground</td>
    <td style="background: #000000; color: #ffffff">#000000</td>
    <td>black</td>
    <td>Very dark color with a good contrast to all other colors.</td>
    <td>border of elements and edges</td>
  </tr>
  <tr>
    <td class="side">base color</td>
    <td style="background: #aaccff;">#aaccff</td>
    <td>VOWL blue</td>
    <td>We reuse the color 'general' of VOWL.</td>
    <td>standard fill color of data shapes</td>
  </tr>
  <tr>
    <td class="side">datatype color</td>
    <td style="background: #ffcc33;">#ffcc33</td>
    <td>VOWL yellow</td>
    <td>We reuse the color 'datatype' of VOWL.</td>
    <td>standard fill color of literals</td>
  </tr>
  <tr>
    <td class="side">highlight</td>
    <td colspan="2">see next table</td>
    <td>For each data shape the highlight color is a darker shade of the
        base color of that element.
    </td>
    <td>fill color of the graph elements when selected</td>
  </tr>
  <tr>
    <td class="side">severity</td>
    <td colspan="2">see next table</td>
    <td>Every severity has its own color.
    </td>
    <td>border color of the data shape based on its severity; default severity is violation</td>
  </tr>
</table>
 
## Color Schemas

<table id="tab-color-schemas">
  <tr>
    <th>Color Schema Name</th>
    <th>Base Color</th>
    <th>Highlight</th>
  </tr>
  <tr>
    <td>base color</td>
    <td style="background: #aaccff;">#aaccff</td>
    <td style="background: #1155cc; color: #ffffff">#1155cc</td>
  </tr>
  <tr>
    <td>severity violation</td>
    <td style="background: #e06666;">#e06666</td>
    <td style="background: #981c1c; color: #ffffff">#b7b7b7</td>
  </tr>
  <tr>
    <td>severity warning (light yellow different from datatype color)</td>
    <td style="background: #ffd966;">#ffd966</td>
    <td style="background: #bf9000; color: #ffffff">#bf9000</td>
  </tr>
  <tr>
    <td>severity information</td>
    <td style="background: #93c47d;">#93c47d</td>
    <td style="background: #38761d; color: #ffffff">#b7b7b7</td>
   </tr>
</table>

