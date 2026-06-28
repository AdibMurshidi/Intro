```python
# Python code to generate the interaction plot
import matplotlib.pyplot as plt
import statsmodels.graphics.factorplots as smg
import os

# Assuming df_machine1 is already loaded and preprocessed
# fig, ax = plt.subplots(figsize=(10, 6))
# fig = smg.interaction_plot(
#     x=df_machine1['Pressure'],
#     trace=df_machine1['Temperature'],
#     response=df_machine1['PartResistance'],
#     ax=ax
# )

# ax.set_title("Interaction Plot of Pressure, Temperature on Part Resistance (Machine 1)", fontsize=18)
# ax.set_xlabel("Pressure (Categorical)", fontsize=18)
# ax.set_ylabel("Mean Part Resistance", fontsize=18)
# ax.tick_params(axis='x', labelsize=14)
# ax.tick_params(axis='y', labelsize=14)
# ax.legend(title="Temperature", title_fontsize=16, fontsize=14, loc='best')
# ax.grid(True, linestyle='--', alpha=0.7)
# ax.set_facecolor("white")
# fig.patch.set_facecolor("white")
# plt.tight_layout()

# # Save the plot
# plot_filename = "interaction_plot_machine1.png"
# plot_filepath = os.path.join('media/pics', plot_filename)
# plt.savefig(plot_filepath, dpi=300)
# plt.close(fig)
```